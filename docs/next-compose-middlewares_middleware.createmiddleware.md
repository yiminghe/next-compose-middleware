<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [next-compose-middlewares/middleware](./next-compose-middlewares_middleware.md) &gt; [createMiddleware](./next-compose-middlewares_middleware.createmiddleware.md)

## createMiddleware() function

nextjs middleware factory

**Signature:**

```typescript
export declare function createMiddleware(ms?: MiddlewareMiddleware[]): (req: NextRequest) => Promise<NextResponse<unknown>>;
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

ms


</td><td>

[MiddlewareMiddleware](./next-compose-middlewares_middleware.middlewaremiddleware.md)<!-- -->\[\]


</td><td>

_(Optional)_


</td></tr>
</tbody></table>
**Returns:**

(req: NextRequest) =&gt; Promise&lt;NextResponse&lt;unknown&gt;&gt;

