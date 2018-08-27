---
name: AWS Route 53
x-slug: aws-route-53
description: Amazon Route 53 is a highly available and scalable cloud Domain Name
  System (DNS) web service. It is designed to give developers and businesses an extremely
  reliable and cost effective way to route end users to Internet applications by translating
  names like www.example.com into the numeric IP addresses like 192.0.2.1 that computers
  use to connect to each other. Amazon Route 53 is fully compliant with IPv6 as well.Amazon
  Route 53 effectively connects user requests to infrastructure running in AWS &ndash;
  such as Amazon EC2 instances, Elastic Load Balancing load balancers, or Amazon S3
  buckets &ndash; and can also be used to route users to infrastructure outside of
  AWS. You can use Amazon Route 53 to configure DNS health checks to route traffic
  to healthy endpoints or to independently monitor the health of your application
  and its endpoints. Amazon Route 53 Traffic Flow makes it easy for you to manage
  traffic globally through a variety of routing types, including Latency Based Routing,
  Geo DNS, and Weighted Round Robin&mdash;all of which can be combined with DNS Failover
  in order to enable a variety of low-latency, fault-tolerant architectures. Using
  Amazon Route 53 Traffic Flow&rsquo;s simple visual editor, you can easily manage
  how your end-users are routed to your application&rsquo;s endpoints&mdash;whether
  in a single AWS region or distributed around the globe. Amazon Route 53 also offers
  Domain Name Registration &ndash; you can purchase and manage domain names such as
  example.com and Amazon Route 53 will automatically configure DNS settings for your
  domains.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Check
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/check/master/_listings/aws-route-53/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Route 53 API - Get Checker Ip Ranges
  x-api-slug: 20130401checkeripranges-get
  description: GetCheckerIpRanges still works, but we recommend that you download
    ip-ranges.json, which includes IP address ranges for all AWS services. For more
    information, see IP Address Ranges of Amazon Route 53 Servers in the Amazon Route
    53 Developer Guide.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/check/master/_listings/aws-route-53/20130401checkeripranges-get-openapi.md
- name: AWS Route 53 API - Create Health Check
  x-api-slug: 20130401healthcheck-post
  description: Creates a new health check.To create a new health check, send a POST
    request to the/2013-04-01/healthcheck resource. The request body must include
    a documentwith a CreateHealthCheckRequest element. The response returns theCreateHealthCheckResponse
    element, containing the health check ID specifiedwhen adding health check to a
    resource record set. For information about adding health checksto resource record
    sets, see ResourceRecordSet:HealthCheckId in ChangeResourceRecordSets. If you
    are registering EC2 instances with an Elastic Load Balancing (ELB) loadbalancer,
    do not create Amazon Route 53 health checks for the EC2 instances. When you register
    anEC2 instance with a load balancer, you configure settings for an ELB health
    check, whichperforms a similar function to an Amazon Route 53 health check.You
    can associate health checks with failover resource record sets in a private hostedzone.
    Note the following:Amazon Route 53 health checkers are outside the VPC. To check
    the health of an endpointwithin a VPC by IP address, you must assign a public
    IP address to the instance in theVPC.You can configure a health checker to check
    the health of an external resource thatthe instance relies on, such as a database
    server.You can create a CloudWatch metric, associate an alarm with the metric,
    and then create ahealth check that is based on the state of the alarm. For example,
    you might create a CloudWatchmetric that checks the status of the Amazon EC2 StatusCheckFailed
    metric, add analarm to the metric, and then create a health check that is based
    on the state of thealarm. For information about creating CloudWatch metrics and
    alarms by using the CloudWatch console,see the Amazon CloudWatch User Guide.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/check/master/_listings/aws-route-53/20130401healthcheck-post-openapi.md
- name: AWS Route 53 API - Delete Health Check
  x-api-slug: 20130401healthcheckhealthcheckid-delete
  description: Deletes a health check. Send a DELETE request to the/2013-04-01/healthcheck/health
    check ID            resource.ImportantAmazon Route 53 does not prevent you from
    deleting a health check even if the health check isassociated with one or more
    resource record sets. If you delete a health check and you don'tupdate the associated
    resource record sets, the future status of the health check can't bepredicted
    and may change. This will affect the routing of DNS queries for your DNS failoverconfiguration.
    For more information, see Replacing and Deleting Health Checks in the Amazon Route
    53 Developer Guide.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/check/master/_listings/aws-route-53/20130401healthcheckhealthcheckid-delete-openapi.md
- name: AWS Route 53 API - Get Health Check
  x-api-slug: 20130401healthcheckhealthcheckid-get
  description: Gets information about a specified health check. Send a GET request
    to the/2013-04-01/healthcheck/health check ID             resource. Formore information
    about using the console to perform this operation, see Amazon Route 53 Health
    Checks and DNS Failover in theAmazon Route 53 Developer Guide.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/check/master/_listings/aws-route-53/20130401healthcheckhealthcheckid-get-openapi.md
- name: AWS Route 53 API - Update Health Check
  x-api-slug: 20130401healthcheckhealthcheckid-post
  description: Updates an existing health check.Send a POST request to the /2013-04-01/healthcheck/health
    check ID             resource. Therequest body must include a document with an
    UpdateHealthCheckRequestelement. For more information about updating health checks,
    see Creating, Updating, and DeletingHealth Checks in the Amazon Route 53 Developer
    Guide.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/check/master/_listings/aws-route-53/20130401healthcheckhealthcheckid-post-openapi.md
- name: AWS Route 53 API - Get Health Check Last Failure Reason
  x-api-slug: 20130401healthcheckhealthcheckidlastfailurereason-get
  description: If you want to learn why a health check is currently failing or why
    it failed mostrecently (if at all), you can get the failure reason for the most
    recent failure. Send aGET request to the /Amazon Route 53 APIversion/healthcheck/health
    checkID/lastfailurereason resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/check/master/_listings/aws-route-53/20130401healthcheckhealthcheckidlastfailurereason-get-openapi.md
- name: AWS Route 53 API - Get Health Check Status
  x-api-slug: 20130401healthcheckhealthcheckidstatus-get
  description: Gets status of a specified health check. Send a GET request to the/2013-04-01/healthcheck/health
    check ID/status resource.You can use this call to get a health check's current
    status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/check/master/_listings/aws-route-53/20130401healthcheckhealthcheckidstatus-get-openapi.md
- name: AWS Route 53 API - List Health Checks
  x-api-slug: 20130401healthcheckmarkermarkerampmaxitemsmaxitems-get
  description: Retrieve a list of your health checks. Send a GET request to the/2013-04-01/healthcheck
    resource. The response to this request includes aHealthChecks element with zero
    or more HealthCheck child elements.By default, the list of health checks is displayed
    on a single page. You can control thelength of the page that is displayed by using
    the MaxItems parameter. You can usethe Marker parameter to control the health
    check that the list beginswith.For information about listing health checks using
    the Amazon Route 53 console, see Amazon Route 53 Health Checks and DNS Failover.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/check/master/_listings/aws-route-53/20130401healthcheckmarkermarkerampmaxitemsmaxitems-get-openapi.md
- name: AWS Route 53 API - Get Health Check Count
  x-api-slug: 20130401healthcheckcount-get
  description: To retrieve a count of all your health checks, send a GET request to
    the/2013-04-01/healthcheckcount resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Networking_AmazonRoute53.png
  humanURL: https://aws.amazon.com/route53/
  baseURL: :///
  tags: Amazon Web Services, DNS, API Service Provider, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/check/master/_listings/aws-route-53/20130401healthcheckcount-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.rekognition.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.route.53.stack.network
- type: x-documentation
  url: http://docs.aws.amazon.com/Route53/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/route53/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=87
- type: x-pricing
  url: https://aws.amazon.com/route53/pricing/
- type: x-registrar-policies
  url: https://aws.amazon.com/route53/amazon-registrar-policies/
- type: x-service-health
  url: http://status.aws.amazon.com/
- type: x-service-level-agreement
  url: https://aws.amazon.com/route53/sla
- type: x-sla
  url: https://aws.amazon.com/route53/sla/
- type: x-website
  url: https://aws.amazon.com/route53/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---