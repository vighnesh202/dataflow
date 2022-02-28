<!--
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->

# Welcome to Apache Beam Notebooks!

[Apache Beam](https://beam.apache.org/) is an open source, unified model for defining both batch and streaming data-parallel processing pipelines.

These notebooks assume you have basic knowledge of
[notebooks](https://jupyterlab.readthedocs.io/en/stable/user/notebook.html) and
the [Python programming language](https://python.org). They are designed to help
you learn the Python SDK of Apache Beam. You can build, iteratively augment your
Apache Beam pipelines, and explore the data in PCollections while doing so.

*   [Example 1: Word Count](Examples/01-Word_Count.ipynb) demonstrates a simple
    batch pipeline that counts words from a text file.
*   [Example 2: Streaming Word Count](Examples/02-Streaming_Word_Count.ipynb)
    demonstrates a simple streaming pipeline that counts words from a stream.
*   [Example 3: Streaming NYC Taxi Ride Data](Examples/03-Streaming_NYC_Taxi_Ride_Data.ipynb)
    demonstrates a streaming pipeline that processes a taxi ride data stream.

We also have:

*   A set of [tutorials](Tutorials/0_START_HERE.md) that go through the basic
    operations of Apache Beam with exercises.
*   A [notebook](Examples/Dataflow_Word_Count.ipynb) that shows you how to
    launch a Dataflow job based on
    [Example 1: Word Count](Examples/01-Word_Count.ipynb).
*   A [notebook](Examples/Visualize_Data.ipynb) that shows you how to visualize
    collected PCollection data with native Interactive Beam visualization and
    various third party visualization libraries.
*   A [notebook](Examples/Use_GPUs_with_Apache_Beam.ipynb) that shows you how to
    write a Beam pipeline and run it with GPUs locally and on Dataflow.
    **Note**: you need to
    [create](https://pantheon.corp.google.com/dataflow/notebooks/list/instances)
    your Dataflow Notebooks instance `With 1 NVIDIA Tesla T4` and check the
    option to `Install NVIDIA GPU driver automatically for me` for this example
    to work.
*   A [notebook](Examples/Apache_Beam_SQL_in_notebooks.ipynb) that shows you how
    to write Beam pipeline with Beam SQL, use `beam_sql` magic to iterate your
    Beam SQL development quickly in notebooks, and launch Dataflow jobs with
    Beam SQL from notebooks.

If you have issues using the notebook, check these
[frequently asked questions](faq.md).

If you have any feedback on these notebooks, drop us a line at
beam-notebooks-feedback@google.com.

# Changelog

## 2022-01

### Added

-   New kernel with Beam v2.35.0

### Deprecated

-   Kernels with Beam v2.25.0, v2.26.0 and v2.27.0

## 2021-12

### Added

-   Beam SQL and `beam_sql` magic support (since Beam v2.34.0) with
    [example](Examples/Apache_Beam_SQL_in_notebooks.ipynb)
-   New kernel with Beam v2.34.0

### Updated

-   The [GPU example](Examples/Use_GPUs_with_Apache_Beam.ipynb) now demonstrates
    -   How to launch Dataflow jobs using GPU from notebooks
    -   How to write a Dockerfile and build a custom container with Cloud Build
        from notebooks

## 2021-11

### Added

-   [Interactive Beam](https://cloud.google.com/dataflow/docs/guides/interactive-pipeline-development#visualizing_the_data_through_the_interactive_beam_inspector)
    JupyterLab extension to interactively inspect the state of pipelines and
    data associated with each PCollection
