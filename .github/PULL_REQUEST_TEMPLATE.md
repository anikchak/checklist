## Overview
_Explain the feature overview or bug details_ 
_**Developer** to provide input_

## JIRA issue
_List down the JIRA story/task/bug for which this deployment is needed_
_**Developer** to provide input_

## Have we verified that the code can be rolled back without causing any problem?
_**Developer** to provide input_

## QA Sign off
- [ ] Check the box if QA sign off is required
- If QA sign off is needed
  - [ ] Check the box if the feature been tested in staging
  - [ ] Check the box if the feature been tested for international as well?
- If QA sign off is not needed describe why :
  _**Developer** to provide input_
- [ ] Check the box if you have ensured that unit testcases have been executed corresponding to the changes done and have passed successfully

## Service Component - Database
_Check the boxes against the questions, if you have adhered to the mentioned guidelines_
- [ ] If you have made changes to schema, check the box if you have verified backward compatibility?
- [ ] If you have added a new column, check the box if you have verified that data backfilling in the new column is required or not?
- [ ] Check the box if you have verified the need to add an index to have better query performance?
- [ ] If you have created a new database, check the box if you have verified the statement timeout and idle in transaction threshold for your user

## Service Component - API
_Check the boxes against the questions, if you have adhered to the mentioned guidelines_
- [ ] If you have made changes to existing API contracts, check the box if you have made sure of backward compatibility?
- [ ] If you have made changes to existing API contracts, check the box if you have made sure that dev testing has happened on old versions of the contract as well?
- [ ] In case the API needs to be rate limited, check the box if you have made sure that throttling has been setup?
- [ ] If you have added a new API in OMS/CAG/PAG, check the box if you have made sure that the API routes to correct shard?

## Service Component - App Impact
_Check the boxes against the questions, if you have adhered to the mentioned guidelines_
- [ ] If your changes impact customer or partner app, the check the box if you have ensured doing a round of testing for older app versions
- [ ] If its a new feature then check the box if you have ensured that it is behind a feature flag?
- [ ] If its a new feature then check the box if you have ensured that it will be a staggered roll out?

## Infra level changes
_Call out the infra changes that were involved; if any_
- List the infra changes below:
  _**Developer** to provide input_
- [ ] Check the box if you have verified that the required permissions and privileges have been granted in prod
- [ ] If changes are getting deployed in UAE stack as well, check the box if you have made sure that the infra provisioning has also happened for UAE and you have verified that required permissions and privileges have been granted for UAE prod

## Observability
_List out the observability details_
- List down the datadog links which will be monitored:
  _**Developer** to provide input_
- List down the SRE cloudwatch dashboards which will be monitored
  _**Developer** to provide input_
- List down the PGAnalyze links which will be monitored
  _**Developer** to provide input_
- List down the alerts that needs to be monitored
  _**Developer** to provide input_

## Post Deployment Sign-off
- [ ] Check the box if you have ensured that a rollback did not happen?
- [ ] Check the box if you monitored the required datadog dashboards
- [ ] Check the box if you have monitored the required cloudwatch dashboards
- In case a rollback (includes both automated or code reverts) happened, kindly provide the details on why it happened
  _**Developer** to provide input_
- In case a rollback happened, specify the rollback time
  _**Developer** to provide input_




