# Report to the President on IT Modernization

[Executive Order (EO) 13,800](https://www.whitehouse.gov/the-press-office/2017/05/11/presidential-executive-order-strengthening-cybersecurity-federal) tasks the Director of the American Technology Council (ATC) to coordinate a report to the President from the Secretary of the Department of Homeland Security (DHS), the Director of the Office of Management and Budget (OMB), and the Administrator of the General Services Administration (GSA), in consultation with the Secretary of Commerce (Commerce), regarding the modernization of Federal Information Technology (IT). In accordance with EO 13,800 the IT Modernization report was drafted and submitted to the President.

The ATC and signatory agencies seek to gather feedback from industry and any other relevant stakeholders on the targeted vision and proposed implementation plan for Federal IT Modernization outlined in the draft report. The information received will be grouped into high level themes under the key input areas listed below.  These themes will be provided to the signatory agencies for consideration of potential changes in the vision and implementation plan. The agencies are not requesting or accepting offers at this time. Information received in response to this notice will not be evaluated or considered as an offer.

In particular, the ATC/signatory agencies are interested in responses to the following areas. We also seek any additional information beyond these questions that industry and stakeholder participants believe would assist in our efforts to become better informed of how to modernize the security and functionality of Federal IT, allow the Federal Government to improve service delivery, and focus effort and resources on what is most important to customers of Government services.

**Key questions include:**

1. What are major attributes that are missing from the targeted vision? ([Appendix A](https://itmodernization.cio.gov/report/appendices/data-level-protections/), [Appendix B](https://itmodernization.cio.gov/report/appendices/cloud-security-protections/))

2. What are major attributes that should not be included in the targeted vision? ([Appendix A](https://itmodernization.cio.gov/report/appendices/data-level-protections/), [Appendix B](https://itmodernization.cio.gov/report/appendices/cloud-security-protections/))

3. Are there any missing or extraneous tasks in [the plan for implementing network modernization & consolidation](https://itmodernization.cio.gov/report/network-modernization/)?

4. Are there any missing or extraneous tasks in [the plan for implementing shared services to enable future network architectures](https://itmodernization.cio.gov/report/shared-services/)?

5. What is the feasibility of the [proposed acquisition pilot](https://itmodernization.cio.gov/report/appendices/acquisition-pilot/)?

Comments should be submitted via **[this web form](https://github.com/GSA/modernization/issues/new)** (GitHub account required) or sent to: **[itmodernization@cio.gov](mailto:itmodernization@cio.gov)**.

Relevant comments received may be publically posted [to this repository](https://github.com/GSA/modernization/issues) (along with any included names or affiliations), and comments will be accepted until **20 September 2017**.


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
