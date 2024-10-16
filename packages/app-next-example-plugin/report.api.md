## API Report File for "app-next-example-plugin"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import { AnyRouteRefParams } from '@backstage/frontend-plugin-api';
import { ConfigurableExtensionDataRef } from '@backstage/frontend-plugin-api';
import { ExtensionDefinition } from '@backstage/frontend-plugin-api';
import { FrontendPlugin } from '@backstage/frontend-plugin-api';
import { default as React_2 } from 'react';
import { RouteRef } from '@backstage/frontend-plugin-api';

// @public (undocumented)
const examplePlugin: FrontendPlugin<
  {},
  {},
  {
    'page:example': ExtensionDefinition<{
      kind: 'page';
      name: undefined;
      config: {
        path: string | undefined;
      };
      configInput: {
        path?: string | undefined;
      };
      output:
        | ConfigurableExtensionDataRef<
            React_2.JSX.Element,
            'core.reactElement',
            {}
          >
        | ConfigurableExtensionDataRef<string, 'core.routing.path', {}>
        | ConfigurableExtensionDataRef<
            RouteRef<AnyRouteRefParams>,
            'core.routing.ref',
            {
              optional: true;
            }
          >;
      inputs: {};
      params: {
        defaultPath: string;
        loader: () => Promise<JSX.Element>;
        routeRef?: RouteRef<AnyRouteRefParams> | undefined;
      };
    }>;
  }
>;
export default examplePlugin;

// @public (undocumented)
export const ExampleSidebarItem: () => React_2.JSX.Element;

// (No @packageDocumentation comment for this package)
```