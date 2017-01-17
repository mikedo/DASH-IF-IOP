# WebVTT metadata track with Images

In this proposal, a new AdapationSet specifying a WebVTT file with metadata is used.
One can then use one or more representation corresponding to thumbnails with different resolutions.


    <AdaptationSet id="3" mimeType="text/vtt" contentType="metadata">
      <Role schemeIdUri="urn:mpeg:dash:role:2011" value="thumbnail"/>

    00:00:00.000 --> 00:00:03.999
	{
		"image": "thumb1.jpg"
	}
	
    00:00:04.000 --> 00:00:07.999
	{
		"image": "thumb2.jpg"
	}

The timing mechanism is then the same as is used in HTML 5 track element which means that some browser player engines may automatically trigger the right callback with the structured data as the scrub bar is moved (or at least as the media is played). 










