## Getting Started

### Requirements

- Node 16^ or newer
- Git

To run the repository locally first clone the repository

```bash
git clone git@github.com:ZEE-5/zee5-O11Y-OEASIS.git
```

Install the dependencies and run the development server

```bash
npm install
npm run dev
# or
yarn
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

<br/>

## API Routes

API routes can be accessed on [http://localhost:3000/api/\*](https://localhost://3000/api) <br/>

### GET

[/api/entities](http://localhost:3000/api/entities)<br/>
Get all the entities of type `APMENV=PROD` listed along with there name and guid

[/api/entities/:guid](https://localhost:3000/api/entities/randomfakeguidid)<br/>
Get all the related entities, name, guid and applicationId of the **source**(`calling entities`) and **target**(`called entities`) <br/>
**Parameters**

|   Name | Required |  Type  | Description                                                               |
| -----: | :------: | :----: | ------------------------------------------------------------------------- |
| `guid` | required | string | The guid of the entity for which you need to get the **related** entities |
