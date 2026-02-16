
<script type="text/javascript">
<!-- Snippet code removed for brevity -- copy from main readme --!> {
src: "https://js.monitor.azure.com/scripts/b/ai.2.min.js", // The SDK URL Source
cfg: { // Application Insights Configuration
    connectionString: "InstrumentationKey=INSTRUMENTATION_KEY",
    extensions: [new Microsoft.ApplicationInsights.DebugPlugin()],
        extensionConfig: {
            ["DebugPlugin"]: {
                trackers: [
                    'trackEvent',
                    'trackPageView',
                    'trackPageViewPerformance',
                    'trackException',
                    'trackTrace',
                    'trackMetric',
                    'trackDependencyData',
                    'throwInternal',        // called when a message is logged internally
                    'logInternalMessage',   // called when a message is logged internally
                    'triggerSend',          // called when data is queued to be sent to the server
                    '_sender',              // called when data is sent to the server
                ]
            }
        }
}});
</script>
```

## Configuration

TBD.

| Name | Default | Description |# Microsoft Application Insights JavaScript SDK - Debug Plugin

## [BETA]

[![GitHub Workflow Status (main)](https://img.shields.io/github/actions/workflow/status/microsoft/ApplicationInsights-JS/ci.yml?branch=main)](https://github.com/microsoft/ApplicationInsights-JS/tree/main)
[![Build Status](https://dev.azure.com/mseng/AppInsights/_apis/build/status%2FAppInsights%20-%20DevTools%2F1DS%20JavaScript%20SDK%20web%20SKU%20(main%3B%20master)?branchName=main)](https://dev.azure.com/mseng/AppInsights/_build/latest?definitionId=8184&branchName=main)
[![npm version](https://badge.fury.io/js/%40microsoft%2Fapplicationinsights-debugplugin-js.svg)](https://badge.fury.io/js/%40microsoft%2Fapplicationinsights-debugplugin-js)
[![gzip size](https://js.monitor.azure.com/scripts/b/ext/ai.dbg.2.min.js.gzip.svg)](https://js.monitor.azure.com/scripts/b/ext/ai.dbg.2.min.js.gzip.svg)
[![minified size size](https://js.monitor.azure.com/scripts/b/ext/ai.dbg.2.min.js.svg)](https://js.monitor.azure.com/scripts/b/ext/ai.dbg.2.min.js.svg)

This README is broken down 
these parts go together to explain the reasoning for this plugin's existance and provides
an explaination as to how everything works. Each of these sections will finish with a
bullet-point list that summarizes the section

## Who Should Use This Plugin

This 
