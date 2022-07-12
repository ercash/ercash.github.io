---
title: "Spring REST Service сервисти Spring Boot колдонбостон ишке ашыруу"
date: 2022-07-12T12:29:00-00:00
categories:
  - spring
tags:
  - spring-rest
---
## Spring REST Service сервисти Spring Boot колдонбостон ишке ашыруу 

**Кырдаал**:
Spring Boot менен түзүлгөн REST-сервис, ичине Tomcat Embedded серверди камтыган өз алдынча чуркоочу jar-пакет болуп түзүлөт. 
> **Note**
> өз алдынча чуркоочу jar - a standalone running jar

Эгер бизге REST-сервистин өзү эле керек болуп, мурунтан эле бар болгон Tomcat серверге иштеткибиз келсе кандай кылабыз?

**Чечүү жолу**:

_Бул статьяларды окуп чыгыш керек:_

Spring Web MVC официалдуу баракча [Web on Servlet Stack](https://docs.spring.io/spring-framework/docs/current/reference/html/web.html#spring-web)
MVC орнотуу Spring фреймворктун версиясына жараша болот, xml же программалык (аннотациянын жардамы менен) түрдө орнотсо болот. Бул жерди статья жардамга [1.1. DispatcherServlet](https://docs.spring.io/spring-framework/docs/current/reference/html/web.html#mvc-servlet).

Эске алуучу нерсе бул Spring Bootтагы @RestController стереотип аннотациясы ичине бул эки аннотацияны @ResponseBody жана @Controller камтыйт. Башкача айтканда Controller view эмес ResponceBody кайтарат. 

Бул жерде жакшы мисал келтирилген: [Spring MVC 4.0 RESTful Web Services Simple Example](https://www.programming-free.com/2014/01/spring-mvc-40-restful-web-services.html)
