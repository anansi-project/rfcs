# The Anansi Project

## What is it?

The Anansi Project is an initiative to bring structure and cohesion to the world of metadata for Comic Books, Mangas, and other graphic novels.

The basic premise of this project is that the current state of things is inadequate. There are multiple existing formats (ComicRack, ComicBookInfo, ACBF, CoMet…), but most of them don't have a clear specification and/or governance. The end result is that all producing/consuming applications are forced to support multiple formats, often with different interpretation due to the lack of specification, and with limiting capabilities as none of the format can handle all the use cases.

## How will that work?

The Anansi Project starts with an RFC ([Request For Comments](https://en.wikipedia.org/wiki/Request_for_Comments)) process, to collect feeback from the community.

It will focus on 3 different areas:
1. Target metadata model
2. Metadata containers
3. Metadata sources of truth

When talking about metadata containers, it is important to distinguish between the _WHAT_ and the _HOW_. The _WHAT_ is the information we want to represent, the _HOW_ is the way we store the information.

Let's take for example the ComicRack `ComicInfo.xml` format:
- the _HOW_ is the file format itself, an XML based document
- the _WHAT_ is the various fields that are described in the XML schema. For example, the `StoryArc` element, describing a single Story Arc the comic book belongs to.

### Target metadata model (the WHAT)

Before discussing any implementation details (the _HOW_), we should work our toward a target metadata model which can cater for all the different use cases the community has around metadata.

Using the existing metadata models from the various containers will help to highlight their limitations, and to work toward a better model.

It is important to note that the target metadata model will need to be evolutive, and as such, to be versioned.

A [publicly viewable Google Sheet](https://docs.google.com/spreadsheets/d/1c8Jdu997crtlHzYlCdQ-cAHTfRtSB3eHV4GOhNBVcJM/edit?usp=sharing) serves as the current state of the target data model.

If you want to provide comment about the target data model, create a Github Issue.

### Metadata containers (the HOW)

Metadata containers are numerous, but most of the time those formats have a strong coupling between their data model and container format.

A container format is no more than a mean to serialize data, so it's easier to store alongside the file it relates to.

The idea behind this stream is two-fold:
1. Focus on the existing container formats themselves, but not their data model, to highlight their limitations.
2. Discuss the required properties of an ideal container format.

### Metadata sources of truth

If the first 2 are the _WHAT_ and _HOW_, this one could be considered as the _WHERE_.

In the U.S. Comics world, ComicVine is considered the source of truth for metadata. Other mediums have their own source of reference data.

The idea of this stream is to gather as much information as possible on the various metadata sources, but also about their limitations, whether regarding the data itself, but also about the ownership of that data.

It might be too early to decide on building an open-source metadata source of truth, but that could be the end goal.

## Great! How can I participate?

The Anansi Project is just starting, first with the RFC process. We will use the Github Issues to discuss topics related to the 3 areas of work. Once we have enough information on a topic, it will be consolidated into dedicated Markdown files.