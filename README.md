# Dataset Publishing Platforms (Open Source)

![](./images/data platforms.png)

In order to save anyone else looking for this time, I thought I'd put together a quick Markdown list of dataset publishing platforms. I'm authoring this on **April 17th 2024** while I'm still very much in the process of trying out different solutions. As with all static documentation, this will eventually become outdated (unless I regularly update it!)

This list focuses on open-source and self-hostable tools that are intended for the purpose of creating data access portals **for sharing datasets with the world at large** and reflects what I've found and tested over the past week or so (I haven't slept much...). This list will likely exclude more general data tools intended for other data visibility use-cases (such as internal data libraries).

As anyone looking for the perfect "thing" will quickly discover, there are a multiplicity of potential options out there but (this is arguable) no obvious choice (in the sense that many would regard Wordpress as the "no brainer" CMS for simple blog publishing).

*(I'm open-sourcing my research because ... why not when writing about open source data platforms!)*

Firstly, let me define my idea for what a "data publishing platform" might look like:

## **Features I Consider Essential** For Open Data Publishing 

- **It's intended for publishing datasets for unrestricted access:** Think government data web portals and the like. 
- **It's got a backend**: This is probably a "me" requirement. I can't imagine maintaining a data portal without some kind of backend that's fairly easy to use. [JKAN](https://jkan.io/) is an interesting looking project but (for me) fell down on this criteria.
- **It's intended for this purpose: ** If you go searching for "data publishing platforms" this is where everything gets a bit confusing. There are more platforms intended for internal data visibility than there are pure-play data publishing platforms. One could share data from a Wordpress site. But (a personal philosophy): in the age of an open source project for almost everything, it seems a pity to use a generalist tool when one honed in on this purpose might exist.

## **Features I Consider Useful** / Nice To Haves

The lack of these isn't a deal-breaker (for me) but I suggest that they bring a huge amount of additional functionality for those potentially interested in looking at your data:

- **Hosted data visualizations**: The ability to embed data visualisations and create them (some - probably me - feel that it's better to separate data visualisation and publishing into separate tools)
- **Data library:** Certain functionalities and features are customary in the world of open data publishing like data libraries describing the fields in the datasets published.

## The "Big Two": CKAN and DKAN

The "big two" in this world (this is my term!) are:

- [CKAN](https://ckan.org/)
- [DKAN](https://www.drupal.org/project/dkan)

The only reason I kept looking beyond the "big two":

- Neither is that easy to install 
- DKAN is attached to the Drupal ecosystem and it's perfectly reasonable not to want to use Drupal

More honestly: they both seem like great tools but neither quite did it for me in terms of ease of use and setup. 

Reason 2: The user-base for data publishing platforms is biased towards large publishing entities like government bodies. Organisations like these can devote a lot of time and resources to mastering a tool and deploying a great instance (or offloading management to an MSP). But not everyone looking to publish datasets has those kind of resources. 

## The Other Tools (A Longish Tail)

And here's the rest of them. It's not as long a list as you might hope. My notes are in the column.

| Project                             | Link                   | Installation Guide                                   | Notes                                                        |
| ----------------------------------- | ---------------------- | ---------------------------------------------------- | ------------------------------------------------------------ |
| Magda                               | https://magda.io/      |                                                      | Seems like a nice platform and they mention one deployment that used the tool specifically for open access data publishing. The dealbreaker for me was that the preferred installation method seemed to involve Terraform/Helm/Kubernetes. If that doesn't phase you, worth checking out. |
| Dataverse                           | https://dataverse.org/ | https://guides.dataverse.org/en/latest/              | Nice looking project intended for creating open source research data publishing libraries (not quite what I had in mind but ... close) |
| Geoserver                           | https://geoserver.org/ | https://docs.geoserver.org/                          | Specifically for sharing geospatial data                     |
| JKAN                                | https://jkan.io/       |                                                      | No backend. Seems to be intended more as a proof of concept engine. |
| Open Data Catalog (Old!)            |                        | https://github.com/opendataphilly/Open-Data-Catalog  | Seemed like a promising initiative but (at the time of writing) there have been no commits in more than a decade. Use very old unmaintained software at your own peril! |
| Datasette                           |                        | https://datasette.io/                                | Very much worth checking out! This platform seems to be picking up momentum. It's specifically intended for sharing and visualising data with a data journalism audience. |
| Open Data Repository Data Publisher |                        | https://github.com/OpenDataRepository/data-publisher | "The Open Data Repository's Data Publisher aims to create a simple tool for publishing data to the web. The project will allow non-technical users to design web layouts and their underlying database structures through a web-based, intuitive interface." |
| Datahub (Opensource)                |                        | https://datahub.io/opensource                        | Will update details if I can get them. The link on their site didn't work so I didn't check further. Looks to be the open source branch of a commercial offering. |
| Invenio Framework                   |                        | https://inveniosoftware.org/products/framework/      | If you want to play with the big boys, this might be the tool for you. I tried and failed to get this running on a VPS (you're telling me that my Digital Ocean droplet wasn't good enough to host something built by CERN!?). This looks like a powerful platform worth considering if you have the ability to configure it. |



This isn't an exhaustive list but should be a somewhat decent guide to some of the obvious options out there at the time of writing (note: there are SaaS/commercial platforms also, as mentioned)

If you're similarly zoned in on this space, this repository from the Open Data Institute is worth keeping an eye on:

https://github.com/theodi/data-publish-list
