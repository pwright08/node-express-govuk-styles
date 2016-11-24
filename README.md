# GOV.UK styles example express application

Example Express application showing how to incorporate the [govuk template and elements](https://www.gov.uk/service-manual/design/using-the-govuk-template-frontend-toolkit-and-elements).

This application was generated using the `express` command, with various assets taken from the [govuk prototype kit](https://github.com/alphagov/govuk_prototype_kit).

Other changes were taken from [APVS production example](https://github.com/ministryofjustice/apvs/tree/develop/alpha/production-example-web) and [APVS external web](https://github.com/ministryofjustice/apvs-external-web). 

Changes that were made to the default express app:

1. Node modules installed:
   * `govuk_template_jinja`
   * `govuk-elements-sass`
   * `express-nunjucks`
2. Add html views including `layout.html` and `includes` folder
3. Update app.js to:
   * Use correct template types and templating engine
   * Pass variables into views
   * Make public folder is accessible in app.js
4. Generate and copy assets from govuk node modules (e.g. by using gulp)

# Run

1. `npm install`
3. `gulp generate-assets`
2. `npm start`
