junit_tests(name='scala',
  dependencies=[
    '3rdparty/jvm/junit',
    '3rdparty/jvm/org/scalatest',
    '3rdparty/jvm/org/specs2',
    'finatra/httpclient',
    'finatra/httpclient/src/test/scala:test-deps',
    'finatra/utils:tests',
    'finatra/http',
    'finatra/inject/inject-app:test-deps',
  ],
  sources=globs(
    'com/twitter/finatra/httpclient/*.scala')
)


scala_library(name="test-deps",
  provides = scala_artifact(
    org = 'com.twitter.finatra',
    name = 'httpclient-test-jar',
    repo = artifactory,
  ),
  dependencies=[
    'finatra/httpclient',
    'finatra/utils:test-deps'
  ],
  sources=globs(
    'com/twitter/finatra/httpclient/test/*.scala'
  ),
)