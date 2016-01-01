# Введение #

В файле main.js, который является частью FBE, находятся JScript-функции, которые вызываются из CPP-кода и доступны также из любого пользовательского скрипта.


# Список #
function FillCoverList() - функция состоит из вызова FillLists().



function apiGetBinary(id)



function apiAddBinary(fullpath, id, type, data)



function GetImageData(id) - отдает base64data вложения с идентификатором id.



function HighlightBorder(element, override, style, width, color)



function ShowPrevImage(source) - выводит эскиз картинки-вложения. Вызывается при наведении указателя мыши на значок просмотра на странице Description. Параметр source - адрес картинки.



function HidePrevImage() - убирает эскиз картинки-вложения.



function ShowFullImage(source)



function LoadXSL(path, lang)



function TransformXML(xslt, dom)



function ShowDescElements()



function LoadFromDOM(dom, lang)



function XmlFromText(text)



function recursiveChangeNbsp(elem, repChar)



function apiLoadFB2(path, lang)



function apiShowDesc(state)



function apiRunCmd(path) – загружает в тег 

&lt;script id=userCmd&gt;

 скрипт, путь к которому передан в аргументе path, после чего вызывает функцию Run() (которая, по идее, описана в файле скрипта).



function apiGetClassName(path)



function apiGetTitle(path)



function apiProcessCmd(path)



function SetInFrame(range, tagName, className)



function RemoveOuterTags(node)



function apiCleanUp(className)



function apiCheckRunnableScript() - возвращает true, если функция Run определена в текущем окне, false в  обратном случае.



function apiSetFastMode(fast)



function   MsgBox(str) - выводит окошко с сообщением str и кнопкой «ОК».



function AskYesNo(str) - выводит окошко с сообщением str и кнопками "Да" и "Нет". Возвращает true, если была нажата кнопка "Да", и false, если "Нет".



function errorHandler(msg,url,lno)



function errCantLoad(xd,file)



function FillImageList(list, bin\_objects)



function FillLists()



function SelectLanguages()



function NewDocumentID()



function PutSpacers(obj)



function InitFieldsets()



function SetDocumentVersion(desc)



function SetProgramUsed(desc)



function SetCurrentDate(desc)



function SetupDescription(desc)



function InflateIt(elem) - для всех абзацев, вложенных в элемент elem (не обязательно непосредственно), вызывает external-функцию, которая делает так, что абзац отображается, даже если он пустой. Нужно для отображения empty-line.



function GetGenre(d)



function dClone(obj)



function Remove(obj)



function Clone(obj)



function ChildClone(obj)



function Indent(node,len)



function SetAttr(node,name,val)



function MakeText(node,name,val,force,indent)



function MakeAuthor(node,name,dv,force,indent)



function MakeDate(node,d,v,indent)



function MakeSeq2(xn,hn,indent)



function MakeSeq(xn,hn,indent)



function IsEmpty(ii) - если ii не null, имеет хотя бы один сыновний элемент, и все сыновние элементы ii являются имеют свойство baseName, равное "empty-line", возвращает true. В противном случае возвращает false.



function MakeTitleInfo(doc,desc,ann,indent)



function IsAuthorExist(node,name,dv)



function IsTextExist(val)



function IsSeqExist2(xn,hn)



function IsSeqExist(xn,hn)



function IsSTBFieldTextExist(sti,desc,doc)



function MakeSourceTitleInfo(doc,desc,ann,indent)



function MakeDocInfo(doc,desc,hist,indent)



function MakePubInfo(doc,desc,indent)



function MakeCustInfo(doc,desc,indent)



function MakeStylesheets(doc,indent)



function GetDesc(doc,ann,hist)



function GetBinaries(doc)



function PutBinaries(doc)



function KillDivs(e)



function GoTo(elem) - функция устанавливает область видимости главного окна редактора на элемент elem.



function SkipOver(np,n1,n2,n3) - возвращает первый элемент, начиная с np и переходя на nextSibling, имеющий имя тега и класс, не равные n1, n2 или n3. Если такого элемента нет, возвращает null. Любой из параметров n1, n2, n3 может отсутствовать.



function StyleCheck(cp,st)



function SetStyle(cp,check,name)



function StyleNormal(cp,check)



function StyleTextAuthor(cp,check)



function StyleSubtitle(cp,check)



function StyleCode(check, cp, range)



function IsCode(cp) - если элемент cp вложен в элемент SPAN с классом code, возвращает true, в противном случае false.



function TextIntoHTML(s) – возвращает строку s, заменив в ней "<" на "&lt;", ">" на "&gt;" и "&" на "&amp;".



function AddTitle(cp, check)



function AddBody(check)



function GetCP(cp)



function InsBefore(parent,ref,item) - если ref не null, вставляет элемент item перед элементом ref, в противном случае вставляет элемент item последним сыновним элементом parent.


function InsBeforeHTML(parent,ref,ht) - если ref не null, вставляет html-код ht перед открывающим тегом элемента ref, в противном случае вставляет html-код ht перед закрывающим тегом элемента parent.



function CloneContainer(cp,check)



function InsImage(check, id) - вставляет "блочную" картинку в книгу, если check!=true. При параметре check==true только проверяет, можно ли в текущий момент вставить блочную картинку. Параметр id - имя картинки (без "fbw-internal:#").



function InsInlineImage(check, id) - вставляет инлайн-картинку в книгу, если check!=true. При параметре check==true только проверяет, можно ли в текущий момент вставить инлайн-картинку. Параметр id - имя картинки (без "fbw-internal:#").



function AddImage(cp, check)



function AddEpigraph(cp,check) - при параметре check==true проверяет, можно ли вставить эпиграф. При других значениях check вставляет эпиграф. В cp передается элемент, содержащий текущее выделение полностью.



function AddAnnotation(cp, check) - при параметре check==true проверяет, можно ли вставить аннотацию книги. При других значениях check вставляет аннотацию книги. В cp передается элемент, содержащий текущее выделение полностью.



function AddTA(cp,check)



function IsCtSection(s) - возвращает false, если элемент s имеет хотя бы один непосредственно сыновний элемент P. В противном случае true.



function FindSE(cp,name)



function MergeContainers(cp,check)



function RemoveOuterContainer(cp,check)



function ImgSetURL(image,url)



function SaveBodyScroll() - сохраняет позицию вертикальной прокрутки окна редактора в переменную document.ScrollSave.



function SetExtendedStyle(elem, button\_id, change)



function ShowElement(id, show)



function ShowElementsMenu(button)