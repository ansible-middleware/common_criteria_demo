# common_criteria-demo
[![CI](https://github.com/ansible-middleware/common_criteria_demo/actions/workflows/ci.yml/badge.svg)](https://github.com/ansible-middleware/common_criteria_demo/actions/workflows/ci.yml)

This is a demo of [common_criteria](https://galaxy.ansible.com/middleware_automation/common_criteria) collection.

## How to use devfile to setup your dev environment

To use the `devfile.yaml` and set up your development environment with OpenShift Dev Spaces or Visual Studio Code, follow these steps:

1. **Clone the Repository**

    ```sh
    git clone https://github.com/ansible-middleware/common_criteria_demo.git
    cd common_criteria_demo
    ```
2. **Install OpenShift Dev Spaces or Visual Studio Code**

    - Download and install [OpenShift Dev Spaces](https://access.redhat.com/products/red-hat-openshift-dev-spaces), else you can directly use Dev Spaces from [Red Hat Developer Snadbox](https://console.redhat.com/openshift/sandbox) as well.
    - Download and install [Visual Studio Code](https://code.visualstudio.com/).

3. 1. **Open the Red Hat Dev Spaces(If you Red Hat subscription use this)**

    - Select `Red Hat Dev Spaces` option from above provided Red hat Developer Sandbox link.
    - Put [common_criteria_demo](https://github.com/ansible-middleware/common_criteria_demo.git) Git repo URL in the `Import from Git` option and click on `Create & Open`.

    2. **Open the Project in Visual Studio Code**

    - Open Visual Studio Code.
    - Open the project folder you cloned: `File > Open Folder...` and select the project directory.
    - Once the folder is open, click on the green button in the bottom-left corner (`><`) and select `New Dev Container`.

Both options will use the `devfile.yaml` to configure and start the development container. You can then start coding and run the playbook within this environment, without worrying about the prerequisite setup.

## Set up
The following sections describe the steps necessary to prepare your machine for execution

First, you'll need to install the collection from middleware_automation and their dependencies:

* [wildfly](https://github.com/ansible-middleware/wildfly)
* [jws](https://github.com/ansible-middleware/jws)
* [common_criteria](https://github.com/ansible-middleware/common_criteria)

Install via:

    $ ansible-galaxy collection install -r requirements.yml

## License

Apache License v2.0 or later

See [LICENSE](LICENSE) to view the full text.
