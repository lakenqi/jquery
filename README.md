# jquery.drag.tag-ul
var example = {
					containerClassName: '可拖拽区域的类名，只能是类名，必填，格式为‘.className’',  //only for className
					sourceArea: {
						name: '源区域的idName/className，必填', //drag elemets source area for className idName
						type: '源区域的类型：id/class，必填', //source area attr for 'class', 'id'
					},
					targetArea: {
						name: '目标区域：idName/className，必填', //drag elements target area for className idName 
						type: '目标区域的类型：id/class，必填', //target area attr for 'class', 'id'
						isLimitedMove: '是否有拖动数量限制，默认false，当为true时，以下两项值必填', //if have,for some fileds, have some tagnums limit
						limitedMaxNums: ['拖动数量最大数，数组形式，如果有超过1个值，需要与limitedIdNames一一对应'], //if have, tag max nums
						limitedIdNames: ['受限制的拖动目标区域idName,数组形式,可共用一个limitedMaxNums值，如果有多个，需要一一对应'], //if have,drag elements target fileds idName, for specail thing for className id or tagName
					},
					CssForDrag: {
						limitedClass: '限制拖动的Css类名称，isLimitedMove为true时，必填', //if have, limited CSS
						targetAreaMoveColor: '拖拽时目标区域高亮颜色，默认blue', //if have, target area backgroundColor when moving the tags
						targetAreaNormalColor: '拖拽结束目标区域恢复原来颜色，默认white', //if have,target area backgroundColor when move over
						movingTagClass: '从源区域拖拽时的标签样式，选填', //if have, when a tag is moving, its CSS				
					},
					callbackFn: '拖拽结束时，回调函数名称，需输入整个函数名称，如function(param),字符串形式,选填', //if have ,when drag over, do some other function; 
				};
