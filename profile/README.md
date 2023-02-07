## Welcome to the SITES community!

Learn about SITES (Swedish Infrastructure for Ecosystem Science) on our [website](https://www.fieldsites.se/).

The SITES data services are developed in collaboration with [ICOS Carbon Portal](https://www.icos-cp.eu/), and the open source code can be found on their [repository](https://github.com/ICOS-Carbon-Portal/).
The [data portal](https://data.fieldsites.se/portal/) hosts our data. It is based on 3 projects:
- [meta](https://github.com/ICOS-Carbon-Portal/meta) handles our metadata.
- [data](https://github.com/ICOS-Carbon-Portal/data) processes and provides access to the data.
- [cpauth](https://github.com/ICOS-Carbon-Portal/cpauth) takes care of user authentication.

### Data upload

Authorised users can upload files to the data portal using either:

#### 🧑‍🔧 Manual uploads

You can upload files manually with [the upload form](https://meta.fieldsites.se/uploadgui/). This method is ideal for single files.

#### ⚙️ Automatic uploads

You can upload files automatically with two [HTTP calls](https://github.com/ICOS-Carbon-Portal/meta#upload-instructions-scripting). This method is ideal to upload multiple files, scheduled uploads (daily for example), or large files. You first create the metadata by posting a [metadata package](https://github.com/ICOS-Carbon-Portal/meta#registering-the-metadata-package). You then [post the data file to the returned URL](https://github.com/ICOS-Carbon-Portal/data#instruction-for-uploading-icos-data-objects).

Before uploading its metadata, you can [test if a file complies to a given data type](https://github.com/ICOS-Carbon-Portal/data#trying-ingestion).

Finally, upload scripts can be written to automate this process. Some examples are available, among other things, in [the scripts repository](https://github.com/fieldSITES/scripts).
