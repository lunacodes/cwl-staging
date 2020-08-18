<h2 id="Implementations" class="section">Implementations <a href="https://www.commonwl.org/#Implementations">§</a></h2>

In Production:

{: .table.table-striped }
|Software|Description|Platform support|
|--- |--- |--- |
|cwltool|Reference implementation of CWL|Linux, OS X, Windows, local execution only|
|Arvados|Distributed computing platform for data analysis on massive data sets. Using CWL on Arvados|AWS, GCP, Azure, Slurm|
|Toil|Toil is a workflow engine entirely written in Python.|AWS, Azure, GCP, Grid Engine, HTCondor, LSF, Mesos, OpenStack, Slurm, PBS/Torque|
|CWL-Airflow|Package to run CWL workflows in Apache-Airflow (supported by BioWardrobe Team, CCHMC)|Linux, OS X|
|REANA|RE usable ANAlyses|Kubernetes, CERN OpenStack (OpenStack Magnum)|

Partial implementations:

{: .table.table-striped }
|Software|Description|Platform support|
|--- |--- |--- |
|Galaxy|Web-based platform for data intensive biomedical research.|yo|
|cwl-tes|CWL engine backended by the GA4GH Task Execution API|Alicloud, AWS, Google, HPC, Local, Spark, TES|
|Xenon|Run CWL workflows using Xenon|any Xenon backend: local, ssh, SLURM, Torque, Grid Engine|
|Consonance|orchestration tool for running SeqWare workflows and CWL tools|AWS, OpenStack, Azure|
|AWE|Workflow and resource management system for bioinformatics data analysis.|yo|
|yacle|Yet Another CWL Engine|local|
|Calrissian|CWL Engine built for Kubernetes|Kubernetes|
|Cromwell|Cromwell workflow engine|Google, HTCondor, Local, LSF, PBS/Torque, SGE, Slurm, TES|
|CWLEXEC|Apache 2.0 licensed CWL executor for IBM Spectrum LSF, supported by IBM for customers with valid contracts.|IBM Spectrum LSF 10.1.0.3+|


