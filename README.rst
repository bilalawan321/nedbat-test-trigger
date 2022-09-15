This repo is part of a test of triggering actions across organizations.

Contact @nedbat with questions.

This repo has a workflow called `trigger.yml`_ that can run on any desired
trigger. It's currently set to run on ``push`` or ``workflow_dispatch``.

It triggers a ``workflow_dispatch`` event in the `build.yml`_ workflow in a
private edX repo called `nedbat-test-trigger-build`_.

This repo has a secret created called ``EDX_BUILD_TOKEN`` which is a
personal access token with ``repo`` scope from someone with access to the
private repo.  The current secret is by nedbat.

.. _trigger.yml: https://github.com/openedx/nedbat-test-trigger/blob/main/.github/workflows/trigger.yml
.. _build.yml: https://github.com/edx/nedbat-test-trigger-build/blob/main/.github/workflows/build.yml
.. _nedbat-test-trigger-build: https://github.com/edx/nedbat-test-trigger-build
