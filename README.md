# FREELANCE LANDING PAGE MVC

La presente plantilla se enfoca en el uso de buenas prácticas con el módelo de arquitectura MCV

## Controllers

El controlador controller.template.php, se encargara de llamar a la plantilla principal.

ejemplo de codigo:

```_code
<?php

class TemplateController
{
  //MAIN VIEW TEMPLATE
  public function index()
  {
    include 'views/template.php';
  }

  //main route url
  static public function path()
  {
    if (!empty($_SERVER["HTPPS"]) && ('on' == $_SERVER["HTTPS"])) {
      return "https://" . $_SERVER['SERVER_NAME'] . '/';
    } else {
      return "http://" . $_SERVER['SERVER_NAME'] . '/';
    }
  }
}

```
