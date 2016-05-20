<!-- title: Gi2Et Installation -->

# Installation

Gi2Et is based on the <a href="https://frappe.io">Frappe Framework</a>, a full stack web framework based on Python, MariaDB, Redis, Node.

To intall Gi2Et, you will have to install the <a href="https://github.com/frappe/bench">Frappe Bench</a>, the command-line, package manager and site manager for Frappe Framework. For more details, read the Bench README.

After you have installed Frappe Bench, go to you bench folder, which is     `frappe.bench` by default and setup **gi2et**.

    bench get-app gi2et {{ source_link }}

Then create a new site to install the app.

    bench new-site mysite

This will create a new folder in your `/sites` directory and create a new database for this site.

Next, install gi2et in this site

    bench --site mysite install-app gi2et

To run this locally, run

    bench start

Fire up your browser and go to http://localhost:8000 and you should see the login screen. Login as **Administrator** and **admin** (or the password you set at the time of `new-site`) and you are set.

<!-- jinja -->
<!-- autodoc -->