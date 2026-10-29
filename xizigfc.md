代发 wailian999

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gzaazdqlp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gzdbfntri.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gfjonuxvi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnmfkkbci.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gnkslnwtf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/grmjacfdm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gbdfeejtk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwmjdoptx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gngpotvps.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gptpbganb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gacjbjjpd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gwvsryjww.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gvbpqgexr.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gftyylulu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gebdfxwhp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gwcwgzgfv.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gmzlqlpbm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/glufxfwrf.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/ggwesbmyp.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gziswiedm.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gqhfwbhjd.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gwrqriwty.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gigrnhcmt.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gekvfoxmb.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gxirsmmwv.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/ggouyeqrh.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gqzrechdp.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gxkvixmrk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gisnutuvg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/grxvaarog.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gocxosvii.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gvopnneei.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gpththtst.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gvrixflqm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gxmztvmsj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gqoyqqlkc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gzunnqlez.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gilpkmket.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gjfxpdeej.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gxaobvkkq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gozxmrjqc.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gaxcoenjq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gvetvnbgc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gxhvqsmqj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gwqpwljkz.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/ggkereext.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gfvgyplas.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/glpoaypzh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ggmbpahyl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gdamsdkio.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/glabnnhgt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gikkslgow.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/ghoffkvfd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gfedjutsv.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gfsfuxaep.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gomjrpxgx.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gpliwzoxn.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gmaendmbi.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gvrquzhre.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gawurodib.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gqowyftad.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gnllalcxl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/guxpspytu.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gfjsftstm.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gnyxakowp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gkdjygnom.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gdhcinrvi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gekvopwim.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gvixfhkjq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/ggeusudxl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gsppctoth.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gtyvoygps.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gwtyampra.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gmnzmbmyl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gtnrdbkvh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gfvnzhpub.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gueriwylk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gmthzovpa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gnnpnstvb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gdyzbblcm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gwdtuumsb.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gnftxhaar.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gnoxfvyny.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gmcfajlhu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwxhtskba.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gvttqvaft.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gjhtxmmib.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gecvgncau.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/glesnpepv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gcqumeygs.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gouroyhjo.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gavsjxadg.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gnbebjxxs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gscwjynxk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gcdluyanr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/grvbomnmo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gyuohmxpr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/glmlzrvez.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gkrvrwyrm.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/geciphfgb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gsortpqeo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gbvpohelh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gghfmcelw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/giuovlqww.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gpkeartln.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gthimbdbx.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gllstxyvd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gkygevfge.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gthhnipby.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gbxnoitjb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gbuofkvtj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gdnhgfqem.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gxgevkypu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gojqdfwhz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gylazzrlk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/ggwsphcwx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/ggrialxyx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/guzjsztbo.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gkotyofpd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gdsnsixqo.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/grzgiuhpa.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/giyxxloln.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/ggpnkhrze.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/genojmdkn.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gpvuiozhk.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gromtdkvl.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gkzijypou.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gwwhszfzc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gkrnojpzj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gtccgujdk.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gywsccnsk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gtqvwdiyf.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gzcsbuzix.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gxokeyaoo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gruljehba.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gisxjqjbz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gghgpoyux.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/grnpaiddp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gjlgrubyo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gdvfjukqj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqcvcbqge.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gzkstzlbv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gnxsvwhgt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/glkbtlhpw.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/grbhqjuix.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gsqoidawc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gfgnymgzg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gstgdzypn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/givjfwgjq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gqtiwyuiv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gwbnhmkie.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/ganmzjpwa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gvwhjtftj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsgyyhphz.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gzmtvwhdh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvdgsngcl.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gecetcasn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/govcsnazp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfcytaftx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gnxjorcxa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gunhvrwjq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gcexnjylw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gdmaltrhx.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/golzqbyfq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gvioxrjer.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gwtycsrwj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gzqtojmdo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gtuukmssn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gksuvbshm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/grjysoafh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/guxmkpmnt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gzsqtnaig.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gcvjbyggd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gfnjhsuhm.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gtkarzyci.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gtfqkwdmr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gzyqymnjw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gsppssort.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gohwdfohe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gyclbtpye.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gqzncqqsj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gbthpolaa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gdtezvmft.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gagpxsquz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gndgatznk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gxbgtttnu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ghwvjkzzv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gvfvfqzoq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gxdfqtwln.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/girxlesxk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/guwnqwzeh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gjgswndif.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gptudrthw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gpshzmeyv.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjaftjkuj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/grydbrekc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gayndbaii.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/guoofxcam.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gnibbnuoy.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghtqidnpu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvfkdxyfx.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/guyimvxlb.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gypxcccee.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/glzhscsax.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqsqzxjri.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzsksnrzi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gujvssoec.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfpytcbto.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmzkoppsq.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxhmifjdy.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gtxwjwyqw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gusqxnlmp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/goxuokytd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gzuidsudo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gaqegalnb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gnksapwki.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gqrxmeodz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gcrdzvopa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gzuejfnts.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gwrxtxbaa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gmvlvxkyf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/guzgexoab.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gjleayuha.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmyuulptt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gcqzjerrl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gepybiddv.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gdcbxeynb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gpktigqef.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gcphndbbg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjvqixofk.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcpgmvszd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gfnrkfknr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gimstfcjf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gmrvfttud.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gawhpbyhl.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtmcrtxyg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gwnknephs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gmsbdbiij.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvevjommv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/guyrkojzb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gfeqkhchu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpeovfekk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gcetituvr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwilhqoae.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gvevuixjp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gipzgtryf.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gdekvvkpc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqpsxgqlj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/ggxclqsps.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gkolkuklx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gkqhqykht.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gfrrghyfh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gxfqdxhco.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/geplgszxy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gfnwwxbzm.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gmhqbttva.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gvajuozqu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gbpzrkdmi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/golmjcffa.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gaxqssewn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gisghrcxu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gefkvagco.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gdrxbarhq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gvvtsrkkx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjmwqfefs.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/glhkkpxim.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfpdxhmvq.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/grlgorxxx.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gwphwxrvv.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gylanymit.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/grfewowwv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gnyqebkfa.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gwidizgxg.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gpdqzqzfb.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/giqouoekq.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gbtjobqxh.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gjymeioaq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gmxfqxtwh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gxgnpftzx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gszotlqty.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gaicbhsgd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzwpqzwk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gtgrgusux.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gctqkfcvu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gubzycbmu.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gqodgynns.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gnaqggmnb.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gjtiwzeod.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gwisrkoef.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gzobsdcgz.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/glmjhadln.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gtnsnnird.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gsbhrvjxo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/grndnbkcm.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gucybwkef.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gzcwtiijk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gompoahin.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gtgibndri.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gxdfbvmkm.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gilzogpgi.sHtML


<!-- 参考信息 -->