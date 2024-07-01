## API Report File for "next-compose-middlewares"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import type { NextRequest } from 'next/server';
import type { default as React_2 } from 'react';
import { ResponseCookie } from 'next/dist/compiled/@edge-runtime/cookies';

// @public (undocumented)
export type ClientCookies = {
    [key: string]: Omit<ResponseCookie, 'expires'> & {
        expires?: number;
    };
};

// @public (undocumented)
export type CookieOptions = Omit<ResponseCookie, 'expires' | 'name' | 'value'> & {
    expires?: Date;
};

// Warning: (ae-forgotten-export) The symbol "GetSetNextContext" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
export function createNextContext<T>(c: T): GetSetNextContext<T>;

// @public (undocumented)
export function getNextContext(): NextContext;

// @public (undocumented)
export type LayoutFunction = (r: LayoutRequest) => ReturnedRender | Promise<ReturnedRender>;

// @public (undocumented)
export type LayoutRequest = {
    params: Params;
    children: React.ReactNode;
};

// @public (undocumented)
export type MiddlewareFunction = (context: NextContext, next: NextFunction) => Promise<any> | void;

// @public (undocumented)
export interface NextContext {
    // (undocumented)
    req: {
        params: any;
        host: string;
        protocol: string;
        secure: boolean;
        url: string;
        ip: string | undefined;
        get: (k: string) => any;
        header: (k: string) => any;
        text: () => Promise<string>;
        json: () => Promise<any>;
        method: string;
        path: string;
        query: any;
        cookies: any;
        headers: any;
    };
    // (undocumented)
    res: {
        _private: {
            return?: any;
            cookies?: ClientCookies;
            headers: any;
            redirect?: string;
            render?: React_2.ReactNode;
            json?: any;
            status?: number;
        };
        clearCookie: (name: string, options?: Omit<CookieOptions, 'expires' | 'maxAge'>) => void;
        cookie: (name: string, value: any, options?: CookieOptions) => void;
        append: (k: string, v: any) => void;
        set: (...args: [key: string, v: any] | [o: any]) => void;
        get: (key: string) => any;
        redirect: (r: string) => void;
        return: (r: any) => void;
        render: (r: React_2.ReactNode) => void;
        json: (j: any) => void;
        status: (s: number) => void;
    };
    // (undocumented)
    type: 'page' | 'route' | 'action' | 'layout';
}

// @public (undocumented)
export type NextFunction = () => Promise<any> | void;

// @public (undocumented)
export type PageFunction = (r: PageRequest) => ReturnedRender | Promise<ReturnedRender>;

// @public (undocumented)
export type PageRequest = {
    params: Params;
    searchParams: Params;
};

// @public (undocumented)
export type Params = Record<string, string | string[]>;

// @public (undocumented)
export type ReturnedRender = void | React.ReactNode;

// @public (undocumented)
export type RouteFunction = (request: NextRequest, context: {
    params: Params;
}) => any;

// @public (undocumented)
export function withActionMiddlewares(fns: MiddlewareFunction[]): <T extends Function>(action: T) => T;

// @public (undocumented)
export const withLayoutMiddlewares: (fns: MiddlewareFunction[]) => (Layout: LayoutFunction) => LayoutFunction;

// @public (undocumented)
export function withPageMiddlewares(fns: MiddlewareFunction[]): (Page: PageFunction) => PageFunction;

// @public (undocumented)
export function withRouteMiddlewares(fns: MiddlewareFunction[]): (Route: RouteFunction) => RouteFunction;

// (No @packageDocumentation comment for this package)

```