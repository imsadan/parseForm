# parseForm
获取form表单数据，可与table数据结合，一同往后端提交

# example:

<input name="id"/>

var formObj = $("#bsInformationForm").parseForm();
var informationAggregationList = ****;
formObj.bsInformationInput = {};
formObj.bsInformationInput.id = formObj['id'];
formObj.bsInformationInput.code = formObj['code'];
formObj.bsInformationInput.goodsName = formObj['goodsName'];
formObj.bsInformationInput.company = formObj['company'];
formObj.bsInformationInput.description = formObj['description'];

formObj = $.extend(formObj, {'bsInformationAggregationList': informationAggregationList});
