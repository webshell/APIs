({
	auth:function(){return auth({provider:fs('/bin/yoda')})},
/** 
 * @category All
 * @param {string} [sentence] Input sentence to turn into Yoda-speak
 * @methodhttp GET
 */
	'YodaSpeak': function(args, opts) {
		var url = 'https://yoda.p.mashape.com/yoda'
		args = args || {}
		if (args['sentence'] == null) throw new Error('sentence is a required parameter')
		var rgx = new RegExp('\{sentence\}', 'g')
		if (url.match(rgx)) {
			url = url.replace(rgx, args['sentence'])
			if (args['sentence']) delete args['sentence']
		}
		if (url.indexOf('[/sentence]') !== -1) {
			url = url.replace('[/sentence]', '/' + args['sentence'])
			if (args['sentence']) delete args['sentence']
		}
		if (url.indexOf('[/sentence]') !== -1) url = url.replace('[/sentence]', '')
		return http({provider:fs('/bin/yoda'),url:url,method:'GET',params:args}, opts)
	}
})