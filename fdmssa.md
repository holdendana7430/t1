代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlvdnphs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lpyvufss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqofjamv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wvtdybdb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3olmewdeg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3hrrozgvt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3opmbrrwg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fsrscpwa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3yrybmbjx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wevmbsaj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zfbcylpd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fmalihkc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fbnygcga.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yzgkuzrm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hrbilopp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3naaasgms.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kakssurm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mutwabbq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nrmutdmh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kuorwzkf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ijyrazds.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fjmzpcjk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3puvmnflj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aclooyti.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nebmchbu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3etyerrvk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yomfeyok.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tytrmcye.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ywxvtrfm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqqbbxsl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kjbiktyk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sgilqkjm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jphtqcoi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hymynwiy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jnuvhsqt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bxinypqc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3cyvqzeow.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yahmwsap.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bfjtqugy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3oppgorlw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tfzusgcp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ziyjihky.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bpppvkti.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3dpxbyatm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jhgrtejl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3urppszsd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dtxlcjbe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vldoesmx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3moycdfgv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jlhguwgx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ibrbrhgp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pxmhygsh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lcdgjnrh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tjroymqm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3talrymlb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pogbcnup.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3obgfpmmi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ccbudjsl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kngzysmh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tmbiwvfx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bibpzfcn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3pozcoodh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3coatrumr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ssavnwik.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rhxgjnpo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3mdbsbkax.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kigqzgvk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ctqdxfqd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dggueiec.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3doafgpzi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ybabvknn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wcujiiig.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3myqtzfwd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zaozqxdr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3etjllbyc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3odjvynvp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ludovqer.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jvztmqcp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yheiowpv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gcrmoazg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3liyxvfhw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3wzlcxkqk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mrtruapv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zhnawyis.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xokudshq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nzrefyns.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ycjmpkcl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nnfcowks.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wrzxjwqt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lumfiawr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3azzcwxva.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3umirlwlo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3igtvuupc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vtropgkd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rtpuxrsh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zdwefouc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rpfsygnt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tszclhwm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mzkoxvaf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zitfteso.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3opyjtnhq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qqciwlrn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3guryrkhw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rncgehkz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3afonfoth.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rwdoersz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qtqxctih.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gntwtyzn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3frxrwttt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pqxbscwk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uymnyswx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3sihqekmr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3psefsobg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3cmrlqsth.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3itlqkyzq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gaypsicr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hrriedmb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ssemhrzv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3cyakokat.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmxgudcg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wdehijhk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cziqhdgi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jdculksk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3apteclye.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3lzvmpiyg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3euaratgk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3agiiuywg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3invctuly.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vhdxvayd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fdvgctsz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tiepcgub.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jlvbcdby.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xoevorrr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kuwyzpgh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3wlwbjsai.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcxxkrqp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3tcojzexh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vlalstod.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gjebeqdr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3msmveyck.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3pndmbcyr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3oydbariy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jcmglxfc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dykxnwtq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xvrxswni.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lxgbdrod.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lapybmbz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3kudomdlz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wrtavkho.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ffmulzuy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhftrqiu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rbfelmni.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3edqgmcyf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3quwvtebo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mawxieqc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zctlfzye.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hxdksata.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ecftpanf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3dgjtwlts.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gqoyruxh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hhyqcljp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ieyzvrhf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uvoydbzi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3antsigbm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ycgzzpwf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jwzjejuf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hejkigzl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3huzghqug.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mfladbwv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ojtnlrov.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zdrmekgg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3neywwvpy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3enifbsfb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dgpkyykm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3dkjurgvn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3sphrdtsv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3lznnvzri.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ercqozbo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lmsegrjv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mruejrxy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kgbjcyzq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kfvyzpuh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzfnqkvi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ejuopgxe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3gxxcomce.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ufsrzgxz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3foctxqas.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dqhyzbdb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pwmuubht.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dduoposl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hivdtprc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ppiwhrsb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3lyejuwlh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3omurzpht.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kdhwuiro.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nbqymnxq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hswijzmz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vrifpzum.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3tfcuhyen.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jjhkizql.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jhcaiayf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oryoasqo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fyprltpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmzcmhzs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rmihqvcn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3uxesgzat.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qfgthksr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pxhlrxox.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qximevht.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3csgkdttf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3elahnlwi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kkuqqcfc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vjdnmzoy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzrmkors.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3owxtpqgd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3newwgnbn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjnavpkm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tivvbezg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zkntvoxv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3aiwnsbdn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3deoefolj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3eipuicez.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3exskowdg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3mycsxeit.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cwwfzwoe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zhwhfylp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yfdjmdgh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bhpmpdno.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hcqmyool.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qrbqjhbn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3obubvjbd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xmfyoxtg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yhsvdeod.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vexhxhjg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rftakyfi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zxadicca.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bxgujbtp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gamddmpo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3usajmsgv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3aflieuzb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gxclotxd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mlcbpggg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gynoetfm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajaqbvuv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kpyxfgrl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nljyhwzb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ylusxzsj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbwkfale.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihqzpcic.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ftusubxm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3larmsclt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mdktudhw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ilktdcem.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ypmvkdks.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ecezbdqn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pinwhamu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hmkqhhdz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nalqhvtb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3mxdvsljd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jvrhgict.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3afbdfhbf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rjkdxwzq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wrmpspru.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3txyoowbx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3bbuadohm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ahfizxfv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cqgosnvb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vbfiygkr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qyjjdwsc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rldmbffm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nlsgyqcs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rhuyslcu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wdnrmnal.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lzdwavou.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xfuzdwei.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3loccndtb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ccuviitp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3umpbmqtm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zaiginfr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ryckvevo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nksdubwr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mjgkmrlo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fmzhpoph.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mogpixky.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3oubleifj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3phihhzgc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgzrvbbi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qlbowlgg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ufdrkckt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfhnlfvp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gauqbxta.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvwwtqzt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lillyzpj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gmdjocbs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqldwtpi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uoqhnoap.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3olxqyszw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qdozzieh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cffezvev.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3arrdftsm.html


<!-- 参考信息 -->