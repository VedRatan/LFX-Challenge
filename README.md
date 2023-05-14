## Description

This test tries to mutate the configmap by adding a label **(lfx-mentorship: kyverno)** to it if the configmap is created in a namespace team-*. For the test to run first of all create a namespace named "team-example".

## Expected Behavior

ConfigMap should be assigned a label **(lfx-mentorship: kyverno)** if it is created in a namespace: team-* , and it should not be assigned a label **(lfx-mentorship: kyverno)** if created in any other namespace for ex: namepace: default is used in this test.