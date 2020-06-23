# Next.js Snippets

Latest snippets for next.js

## Installation

- install the extension
- reload vscode
- snippets will be ready to use

## Page initialization snippets

### `nafe` (nextjs arrow function (export at the end))

```javascriptreact
const FileName = () => {
    return (
        <div>
            ${1:Enter}
        </div>
    );
}

export default FileName;
```

### `naf` (nextjs arrow function)

```javascriptreact
export default () => {
    return (
        <div>
            ${1:Enter}
        </div>
    );
}
```

### `nafe` (nextjs normal function (export at the end))

```javascriptreact
function FileName() {
    return (
        <div>
            ${1:Enter}
        </div>
    );
}

export default FileName;
```

### `nf` (nextjs normal function )

```javascriptreact
export default function ()  {
    return (
        <div>
            ${1:Enter}
        </div>
    );
}
```

## Nextjs snippets

### `ngsspr` (nextjs getServerSideProps)

```javascriptreact
 export const getServerSideProps = async (ctx) => {

    return {
        props:{
            data:null
        }
    }
}
```

### `ngspr` (nextjs getStaticProps)

```javascriptreact
 export const getStaticProps = async (ctx) => {

    return {
        props:{
            data:null
        }
    }
}
```

### `ngspa` (nextjs getStaticPaths)

```javascriptreact
export const getStaticPaths = async () => {

    return {
        paths:[],
        fallback:false
    }
}
```

### `ngipr` (nextjs getInitialProps)

```javascriptreact
FileName.getInitialProps = async (ctx) => {

    return {
        ${3:data:null}
    }
}
```

## Nextjs Custom app and document (\_app.js,\_document.js)

### `ncapp` (nextjs custom app)

```javascriptreact
// import App from 'next/app'

const MyApp = ({ Component pageProps }) => {
    return <Component {...pageProps} />
}
// Only uncomment this method if you have blocking data requirements for
// every single page in your application. This disables the ability to
// perform automatic static optimization causing every page in your app to
// be server-side rendered.

//MyApp.getInitialProps = async (appContext) => {
// calls page's `getInitialProps` and fills `appProps.pageProps`
// const appProps = await App.getInitialProps(appContext);
// return { ...appProps }
// }

export default MyApp;
```

### `ncdocument` (nextjs custom document)

```javascriptreact
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

```javascriptreact
const FileName = () => {
    return (
        <div>
            ${1:Enter}
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

```javascriptreact
function FileName() {
    return (
        <div>
            ${1:Enter}
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

```javascriptreact
const FileName = () => {
    return (
        <div>
            ${1:Enter}
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

```javascriptreact
function FileName() {
    return (
        <div>
            ${1:Enter}
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

```javascriptreact
const FileName = () => {
    return (
        <div>
            ${1:Enter}
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

```javascriptreact
import Link from 'next/link';
```

### `nir` (nextjs import router(default))

```javascriptreact
import Router from 'next/router';
```

### `niur` (nextjs import useRouter)

```javascriptreact
import {useRouter} from 'next/router';
```

### `nih` (nextjs import Head)

```javascriptreact
import Head from 'next/head';
```

## Imported Components Usage

### `nulwhref` (nextjs use link with href)

```javascriptreact
<Link href="path"><a>Value</a></Link>
```

### `nulwas` (nextjs use link with as)

```javascriptreact
<Link href="routepattern" as="path"><a>Value</a></Link>
```

### `nuur` (nextjs use useRouter)

```javascriptreact
const router = useRouter();
```

### `nuh` (nextjs use Head )

```javascriptreact
<Head><title>Title</title></Head>
```
