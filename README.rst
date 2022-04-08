REST API backed by Amazon DynamoDB
==================================

This template provides a REST API that's backed by an Amazon DynamoDB table.
This application is deployed using the AWS CDK.

For more information, see the `Deploying with the AWS CDK
<https://aws.github.io/chalice/tutorials/cdk.html>`__ tutorial.


Quickstart
----------

First, you'll need to install the requirements for the project.

::

  $ python3 -m venv venv

  $ source venv/bin/activate

  $ python3 -m pip install -r requirements.txt

  $ npm --prefix infrastructure install

There's also separate requirements files in the ``infrastructure``
and ``runtime`` directories if you'd prefer to have separate virtual
environments for your CDK and Chalice app.

To deploy the application, ``cd`` to the ``infrastructure`` directory.
If this is you're first time using the CDK you'll need to bootstrap
your environment.

::

  $ npx cdk bootstrap

Then you can deploy your application using the CDK.

::

  $ npx cdk deploy


Project layout
--------------

This project template combines a CDK application and a Chalice application.
These correspond to the ``infrastructure`` and ``runtime`` directory
respectively.  To run any CDK CLI commands, ensure you're in the
``infrastructure`` directory, and to run any Chalice CLI commands ensure
you're in the ``runtime`` directory.
