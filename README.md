# Report to the President on IT Modernization

[Executive Order (EO) 13,800](https://www.whitehouse.gov/the-press-office/2017/05/11/presidential-executive-order-strengthening-cybersecurity-federal) tasks the Director of the American Technology Council (ATC) to coordinate a report to the President from the Secretary of the Department of Homeland Security (DHS), the Director of the Office of Management and Budget (OMB), and the Administrator of the General Services Administration (GSA), in consultation with the Secretary of Commerce (Commerce), regarding the modernization of Federal Information Technology (IT).

In accordance with EO 13,800 the IT Modernization report was submitted to the President.

This repository hosts the web-friendly version of this report.

## Development of the report website itself

If you're using this repository to run the site locally, instructions follow below.

Dependencies:

* **Node 6+** to install USWDS and dependencies
* **Ruby** and **bundler** to install / run Jekyll

##### First-time setup

1. `npm install` to install the USWDS, and Gulp dependencies.
2. `npm install -g gulp` to let you use the `gulp` CLI directly.
3. `bundle install` to install Jekyll.

##### Running the app

If you'll be editing the Sass/CSS:

* `gulp watch`

To run the app:

* `bundle exec jekyll serve`
