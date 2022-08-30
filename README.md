[![Install](https://vsmarketplacebadge.apphb.com/installs-short/pulkitgangwar.nextjs-snippets.svg)](https://vsmarketplacebadge.apphb.com/installs-short/pulkitgangwar.nextjs-snippets.svg)
[![Downloads](https://vsmarketplacebadge.apphb.com/downloads-short/pulkitgangwar.nextjs-snippets.svg)](https://vsmarketplacebadge.apphb.com/downloads-short/pulkitgangwar.nextjs-snippets.svg)
[![Ratings](https://vsmarketplacebadge.apphb.com/rating-star/pulkitgangwar.nextjs-snippets.svg)](https://vsmarketplacebadge.apphb.com/rating-star/pulkitgangwar.nextjs-snippets.svg)

# Next.js Snippets

Latest snippets for next.js

![next js-snippets-gif](https://user-images.githubusercontent.com/50038851/85401251-59c46400-b577-11ea-9eb3-a8ed916c711e.gif)

## Installation

- install the extension
- reload vscode
- snippets will be ready to use

## Language

- [JavascriptReact](#javascript)
- [TypescriptReact](#typescript)

# Javascript

## Page initialization snippets

### `nafe` (nextjs arrow function (export at the end))

```js
const FileName = () => {
    return (
        <div>
            CONTENT
        </div>
    );
}

export default FileName;
```

### `naf` (nextjs arrow function)

```js
export default () => {
    return (
        <div>
            CONTENT
        </div>
    );
}
```

### `nfe` (nextjs normal function (export at the end))

```js
function FileName() {
    return (
        <div>
            CONTENT
        </div>
    );
}

export default FileName;
```

### `nf` (nextjs normal function )

```js
export default function ()  {
    return (
        <div>
            CONTENT
        </div>
    );
}
```

## Nextjs snippets

### `ngsspr` (nextjs getServerSideProps)

```js
 export const getServerSideProps = async (ctx) => {

    return {
        props:{
            data:null
        }
    }
}
```

### `ngspr` (nextjs getStaticProps)

```js
 export const getStaticProps = async (ctx) => {

    return {
        props:{
            data:null
        }
    }
}
```

### `ngspa` (nextjs getStaticPaths)

```js
export const getStaticPaths = async () => {

    return {
        paths:[],
        fallback:false
    }
}
```

### `ngipr` (nextjs getInitialProps)

```js
FileName.getInitialProps = async (ctx) => {

    return {
        ${3:data:null}
    }
}
```

## Nextjs Custom app and document (\_app.js,\_document.js)

### `ncapp` (nextjs custom app)

```js
// import App from 'next/app'

const MyApp = ({ Component pageProps }) => {
    return <Component {...pageProps} />
}

//MyApp.getInitialProps = async (appContext) => {
// calls page's `getInitialProps` and fills `appProps.pageProps`
// const appProps = await App.getInitialProps(appContext);
// return { ...appProps }
// }

export default MyApp;
```

### `ncdocument` (nextjs custom document)

```js
import Document, { Html, Head, Main, NextScript } from 'next/document'

class MyDocument extends Document {
    static async getInitialProps(ctx) {
        const initialProps = await Document.getInitialProps(ctx)
        return { ...initialProps }
    }

    render() {
        return (
            <Html>
                <Head/>
                <body>
                    <Main />
                    <NextScript />
                </body>
            </Html>
        )
    }
}

export default MyDocument;
```

## Nextjs api routes

### `napi` (nextjs api route)

```javascritreact
export default (req,res) => {


}
```

## Nextjs page initialization function with Nextjs functions

### `nafewserver` (nextjs arrow function (export at the end) with getServerSideProps)

```js
const FileName = () => {
    return (
        <div>
            CONTENT
        </div>
    );
}

export const getServerSideProps = async (ctx) => {

    return {
        props:{
            data:null
        }
    }
}

export default FileName;
```

### `nfewserver` (nextjs normal function (export at the end) with getServerSideProps)

```js
function FileName() {
    return (
        <div>
            CONTENT
        </div>
    );
}

export async function getServerSideProps(ctx){

    return {
        props:{
            data:null
        }
    }
}

export default FileName;
```

### `nafewstatic` (nextjs arrow function (export at the end) with getStaticProps)

```js
const FileName = () => {
    return (
        <div>
            CONTENT
        </div>
    );
}

export const getStaticProps = async (ctx) => {

    return {
        props:{
            data:null
        }
    }
}

export default FileName;
```

### `nfewstatic` (nextjs normal function (export at the end) with getStaticProps)

```js
function FileName() {
    return (
        <div>
            CONTENT
        </div>
    );
}

export async function getStaticProps(ctx){

    return {
        props:{
            data:null
        }
    }
}

export default FileName;
```

## Static generation snippet

### `!!static` (initializing function with getStaticPaths and getStaticProps)

```js
const FileName = () => {
    return (
        <div>
            CONTENT
        </div>
    );
}

export const getStaticPaths = async () => {

    return {
        paths:[],
        fallback:false
    }
}

export const getStaticProps = async (ctx) => {

    return {
        props:{
            data:null
        }
    }
}

export default FileName;
```

## Importing Components

### `nil` (nextjs import link)

```js
import Link from 'next/link';
```

### `nir` (nextjs import router(default))

```js
import Router from 'next/router';
```

### `niur` (nextjs import useRouter)

```js
import {useRouter} from 'next/router';
```

### `nih` (nextjs import Head)

```js
import Head from 'next/head';
```

## Imported Components Usage

### `nulwhref` (nextjs use link with href)

```js
<Link href="path"><a>Value</a></Link>
```

### `nulwas` (nextjs use link with as)

```js
<Link href="routepattern" as="path"><a>Value</a></Link>
```

### `nuur` (nextjs use useRouter)

```js
const router = useRouter();
```

### `nuh` (nextjs use Head )

```js
<Head><title>Title</title></Head>
```

# Typescript

## Page initialization snippets

### `nafe` (nextjs arrow function (export at the end))

```js
const FileName = () => {
    return (
        <div>
            CONTENT
        </div>
    );
}

export default FileName;
```

### `naf` (nextjs arrow function)

```js
export default () => {
    return (
        <div>
            CONTENT
        </div>
    );
}
```

### `nafe` (nextjs normal function (export at the end))

```js
function FileName() {
    return (
        <div>
            CONTENT
        </div>
    );
}

export default FileName;
```

### `nf` (nextjs normal function )

```js
export default function ()  {
    return (
        <div>
            CONTENT
        </div>
    );
}
```

## Nextjs page initialization function with Nextjs functions

### `ntsfwserver` (nextjs typescript function with getServerSideProps)

```ts
import {GetServerSideProps} from 'next';

const FileName = () => {
    return (
        <div>
            CONTENT
        </div>
    );
}

export const getServerSideProps:GetServerSideProps = async (ctx) => {

    return {
        props:{
            data:null
        }
    }
}

export default FileName;
```

### `ntsfwstatic` (nextjs typescript function with getStaticProps)

```ts
import {GetStaticProps} from 'next';

const FileName = () => {
    return (
        <div>
            CONTENT
        </div>
    );
}

export const getStaticProps:GetStaticProps = async (ctx) => {

    return {
        props:{
            data:null
        }
    }
}

export default FileName;
```

## Nextjs api routes

### `ntsapi` (nextjs typescript api route)

```ts
import { NextApiRequest, NextApiResponse } from 'next';

export default (req: NextApiRequest, res: NextApiResponse) => {


}
```

## Nextjs Custom app and document (\_app.js,\_document.js)

### `ntscapp` (nextjs typescript custom app)

```ts
import { AppProps } from 'next/app';

const MyApp = ({ Component pageProps }:AppProps) => {
    return <Component {...pageProps} />
}

export default MyApp;
```

### `ntscdocument` (nextjs typescript custom document)

```js
import Document, { Html, Head, Main, NextScript } from 'next/document'

class MyDocument extends Document {
    static async getInitialProps(ctx) {
        const initialProps = await Document.getInitialProps(ctx)
        return { ...initialProps }
    }

    render() {
        return (
            <Html>
                <Head/>
                <body>
                    <Main />
                    <NextScript />
                </body>
            </Html>
        )
    }
}

export default MyDocument;
```

## Static generation snippet

### `!!tsstatic` (initializing function with getStaticPaths and getStaticProps(typescript))

```ts
import {GetStaticPaths,GetStaticProps} from 'next';
const FileName = () => {
    return (
        <div>
            CONTENT
        </div>
    );
}

export const getStaticPaths:GetStaticPaths = async () => {

    return {
        paths:[],
        fallback:false
    }
}

export const getStaticProps:GetStaticProps = async (ctx) => {

    return {
        props:{
            data:null
        }
    }
}

export default FileName;
```

## Importing Components

### `nil` (nextjs import link)

```js
import Link from 'next/link';
```

### `nir` (nextjs import router(default))

```js
import Router from 'next/router';
```

### `niur` (nextjs import useRouter)

```js
import {useRouter} from 'next/router';
```

### `nih` (nextjs import Head)

```js
import Head from 'next/head';
```

### `nii` (nextjs import Image)

```js
import Image from 'next/image';
```

### `nid` (nextjs import dynamic)

```js
import dynamic from 'next/dynamic';
```