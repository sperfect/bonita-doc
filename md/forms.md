# Forms

This page explains how to add a form resource to the Portal and make it available to users. Form resources are intended for use in applications.

Pages are [exported. imported, modified, and deleted](resource-management.md) as resources in Bonita BPM Portal. 

Form definition <!--{.h2}-->

A form is a [page](pages.md) that belongs to a process. It could be a process instantiation form, a human task form, or an overview form. There are some extra things to consider when you are creating a form compared with an ordinary page, concerning how data is passed between the process instance and the form.

A [context](contracts-and-contexts.md) is the set of data provided by the process instance or task instance to the form. 
There is no context for a process instantiation form.

A [contract](contracts-and-contexts.md) is the definition of that data that the form returns to the process instance. There is no contract for an overview form.

Three auto-generated forms are provided by default, for process instantiation, for human task execution, and for the case overview. 

The process instantiation and step execution auto-generated forms are based on the relevant contract and they are a useful tool for testing and debugging your application. 

The overview consists of three main sections:

* List of business data: it shows the content of the business variables used by the case.
* List of documents: it shows the content of each document used by the case.
* Timeline: it shows in chronological order information about all the actions that have been performed in the selected case.

You can see how to manage the link between process and and form in the documenation about [live update](live-update.md)
