Project Nami Blob Cache -- Installation

1)	Create a storage account in the same datacenter as your web site, if you do not have one already.

2)	While in the storage account settings, copy the Primary Access Key

3)	Create a container for cache objects, setting access to Private

4)	Navigate to the Configure tab of your web site, and add the following values to "app settings"

	ProjectNamiBlobCache.StorageAccount		<your storage account name>
	
	ProjectNamiBlobCache.StorageKey			<your storage account Primary Access Key>
	
	ProjectNamiBlobCache.StorageContainer	<your cache container in your storage account>
	
	ProjectNamiBlobCache.Proactive			<set to 1 to enable Proactive mode, otherwise set to 0>
	
	ProjectNamiBlobCache.Debug				<set to 1 to enable debug output in site pages, otherwise set to 0>
	
5)	Be sure to Save your Configuration changes

6)	Upload the project-nami-blob-cache folder into the wp-content/plugins folder of your site

7)	Navigate to Plugins and enable the Project Nami Cache Plugin

8)	Navigate to PN Blob Cache within Settings

9)	Enter the values for your Blob Account and set the Time To Live for cached pages

10)	Build this project, then create a Bin folder at the root of your site and upload the two DLL files produced by the build into the Bin folder.

11)	Copy the provided web.config file into the root of your site, or if you already have a web.config file instead merge the contents into your existing file.


