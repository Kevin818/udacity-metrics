**Note:** For the screenshots, you can store all of your answer images in the `answer-img` directory.

## Verify the monitoring installation
![Alt text](/answer-img/1.kubectl get pods.PNG?raw=true "kubectl get pods")


## Setup the Jaeger and Prometheus source
![Alt text](/answer-img/2.grafana.PNG?raw=true "grafana")
<img src="/answer-img/2.grafana.PNG" alt="grafana" title="grafana">

## Create a Basic Dashboard
![Alt text](/answer-img/3.prometheus.PNG?raw=true "prometheus")

## Describe SLO/SLI
SLOs are clear goals. SLI is quantifiable definition and performance.
For SLO monthly uptime, SLI can be defined as a monthly uptime of 99%.
For SLO request response time, SLI can be defined as 98% of the request response time is within the required time.

## Creating SLI metrics.
| SLO           | SLI           |
| ------------- | ------------- |
| Latency       | request response time |
| Error Rate  | error rate in a time period  |
| Uptime        | the active service has been running |
| Network capacity | Network capacity in a time period  |
| CPU Usage     | Percent of CPU used in a time period  |


## Create a Dashboard to measure our SLIs
![Alt text](/answer-img/4.dashboard.PNG?raw=true "dashboard")

## Tracing our Flask App
*TODO:*  We will create a Jaeger span to measure the processes on the backend. Once you fill in the span, provide a screenshot of it here. Also provide a (screenshot) sample Python file containing a trace and span code used to perform Jaeger traces on the backend service.
![Alt text](/answer-img/6.jaeger1.PNG?raw=true "jaeger")
![Alt text](/answer-img/6.jaeger2.PNG?raw=true "jaeger")


## Jaeger in Dashboards
*TODO:* Now that the trace is running, let's add the metric to our current Grafana dashboard. Once this is completed, provide a screenshot of it here.
![Alt text](/answer-img/7.dashboard2.PNG?raw=true "Jaeger in Dashboards")

## Report Error
*TODO:* Using the template below, write a trouble ticket for the developers, to explain the errors that you are seeing (400, 500, latency) and to let them know the file that is causing the issue also include a screenshot of the tracer span to demonstrate how we can user a tracer to locate errors easily.

TROUBLE TICKET

Name: Error 500

Date: Oct 29 12:52pm

Subject: backend service route "/star"

Affected Area: Backend service 

Severity: Urgent 

Description: went running backend service route "/star" get a error and the service fail


## Creating SLIs and SLOs
- Applications service uptime 
- CPU and memory usage 
- Request and Response time 
- Http Errors (4xx or 5xx error)

## Building KPIs for our plan
![Alt text](/answer-img/8.KPI.PNG?raw=true "KPIs1")
![Alt text](/answer-img/8.KPI2.PNG?raw=true "KPIs2")

## Final Dashboard

![Alt text](/answer-img/9.final.PNG?raw=true "final")


1. CPU And Memory usage 
    - measure the memory and CPU to prevent overloading and excessive use of resources 

2. Services Uptime
    - Watch the uptime of the backend and frontend service to make sure availability

3. Response time
    - watch the services responses 

4. HTTP's Errors 
    - rate the application HTTP's Errors and see if the service API is working correctly 
