<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [next-compose-middlewares](./next-compose-middlewares.md) &gt; [withActionMiddlewares](./next-compose-middlewares.withactionmiddlewares.md)

## withActionMiddlewares() function

create higher order action with middlewares

**Signature:**

```typescript
export declare function withActionMiddlewares(fns: MiddlewareFunction[]): <T extends Function>(action: T) => T;
```

## Parameters

<table><thead><tr><th>

Parameter


</th><th>

Type


</th><th>

Description


</th></tr></thead>
<tbody><tr><td>

fns


</td><td>

[MiddlewareFunction](./next-compose-middlewares.middlewarefunction.md)<!-- -->\[\]


</td><td>


</td></tr>
</tbody></table>
**Returns:**

&lt;T extends Function&gt;(action: T) =&gt; T
