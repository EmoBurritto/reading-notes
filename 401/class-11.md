# Reading Class 11

## Spring App Basics

Spring is a framework. 

Frameworks tackle common application problems. 

Provides pattern and structures for java app. 

Spring framework addresses: 

- handling interraleted depedencies among objects; done by dependency injection

- database connectivity done usually by JDBC; different data access API and connectivity

- Spring MVC; web network connectivity, REST API's

typical Java app is network of objects with references to oen another if applicable. 

Spring’s approach to building web sites, HTTP requests are handled by a controller

Spring Boot Devtools: (use like REACT in JS)

- Enables hot swapping.

- Switches template engines to disable caching.

- Enables LiveReload to automatically refresh the browser.

- Other reasonable defaults based on development instead of production.


(reference: https://spring.io/guides/gs/serving-web-content/)

## Spring MVC and Thymeleaf

Thymeleaf: 

- modern server-side Java template engine that allows the ability to inject varibales from controler to be converted into HTML to create dynamic HTML content 

Spring MVC calls the pieces of data that can be accessed during the execution of views model attributes; equivalent term in Thymeleaf language is context variable

typical Spring MVC application, @Controller classes are responsible for preparing a model map with data and selecting a view to be rendered

To add model attributes:

Add attribute to Model via its addAttribute method:

    @RequestMapping(value = "message", method = RequestMethod.GET)
        public String messages(Model model) {
            model.addAttribute("messages", messageRepository.findAll());
            return "message/list";
        }
Return ModelAndView with model attributes included:

    @RequestMapping(value = "message", method = RequestMethod.GET)
        public ModelAndView messages() {
            ModelAndView mav = new ModelAndView("message/list");
            mav.addObject("messages", messageRepository.findAll());
            return mav;
        }

Expose common attributes via methods annotated with @ModelAttribute:

    @ModelAttribute("messages")
        public List<Message> messages() {
            return messageRepository.findAll();
        }

In Thymeleaf, these model attributes (or context variables in Thymeleaf jargon) can be accessed with the following syntax: ${attributeName}, where attributeName in our case is messages.

To acces request Parameters:

use the param. prefix:

    <p th:text="${param.q}">Test</p>

Session Attributes:

add mySessionAttribute to session:

    @RequestMapping({"/"})
        String index(HttpSession session) {
            session.setAttribute("mySessionAttribute", "someValue");
            return "index";
        }

ServletContext attributes:

use the #servletContext. prefix:

        <table>
                <tr>
                    <td>My context attribute</td>
                    <!-- Retrieves the ServletContext attribute 'myContextAttribute' -->
                    <td th:text="${#servletContext.getAttribute('myContextAttribute')}">42</td>
                </tr>
                <tr th:each="attr : ${#servletContext.getAttributeNames()}">
                    <td th:text="${attr}">javax.servlet.context.tempdir</td>
                    <td th:text="${#servletContext.getAttribute(attr)}">/tmp</td>
                </tr>
            </table>

Spring Beans:

Thymeleaf allows accessing beans registered at the Spring Application Context with the @beanName syntax, for example:

    <div th:text="${@urlService.getApplicationUrl()}">...</div> 

(reference: https://www.thymeleaf.org/doc/articles/springmvcaccessdata.html)
