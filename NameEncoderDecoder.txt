class NameEncoderDecoder {
 
  public String encode(String name) {
     
  String name1 = name.replace("e","1")
  .replace ("u","2")
  .replace("i","3")
  .replace ("o","4")
  .replace ("a","5"); 
    
    return "NOTFORYOU"+name1+"YESNOTFORYOU";
  }
  
  public String decode(String name) {
  String s = name.replaceFirst("NOTFORYOU", "");
  String s1 = s.substring(0, s.indexOf("YESNOTFORYOU"));
    
  return s1.replace("1","e")
  .replace ("2","u")
  .replace("3","i")
  .replace ("4","o")
  .replace ("5","a");
  }  
}