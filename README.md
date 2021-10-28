# rush-repro-peerdep-mess

Reproduction of the issue https://github.com/microsoft/rushstack/issues/2992

# How to repro

1. git clone the repo
2. `rush update --full`

This leads to warnings

````
 WARN  office-ui-fabric-react > @fluentui/react-focus > @uifabric/styling > @fluentui/theme: @uifabric/utilities@7.33.5 requires a peer of react@>=16.8.0 <17.0.0 but none was installed.
 WARN  office-ui-fabric-react > @fluentui/react-focus > @uifabric/styling: @fluentui/theme@1.7.4 requires a peer of react@>=16.8.0 <17.0.0 but none was installed.
 WARN  office-ui-fabric-react: @fluentui/react-focus@7.18.1 requires a peer of react@>=16.8.0 <17.0.0 but none was installed.
 WARN  office-ui-fabric-react: @fluentui/react-window-provider@1.0.2 requires a peer of react@>=16.8.0 <17.0.0 but none was installed.
 WARN  office-ui-fabric-react: @uifabric/foundation@7.10.1 requires a peer of react@>=16.8.0 <17.0.0 but none was installed.

````
