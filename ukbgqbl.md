代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gcruuougw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ggetdxrqs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/giwmngzfa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gcgrpwgym.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gacfcxjgl.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gbwzotyso.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/guyxdomkl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gmplvorxt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gfwyyxkay.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/guvhwmvgx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/guvjfkynn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gewxzkcme.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gkqjlshrg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/goouuaoou.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gnajlhfxn.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gjdnqtnml.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gfbytdwtl.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gvkoshzfz.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gsagcrmde.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gejurkped.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gsxlajxml.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gvvqjdylo.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/godpkgmva.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gcypbkext.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gbwwqetbe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gvfsxhlas.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gbawuenql.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gsxkgsjum.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gjcnroggz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/giyzytbev.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gvumfrcuu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/ggpwvwite.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/ggkfrdewm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gkrwczepy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gxsfycfpz.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/grygmwtxj.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gjbhdkkbm.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gyhziyjdg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/glcdtmfjb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gapcdowbb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gvfhenpen.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gpevugmrc.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gyabojlmp.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gsnesuypz.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gpeqyadez.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gunomypel.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gjkyskfiv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gvjfdvtye.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/geiwdahfr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gyarbahcf.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/geaboehbl.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gvxnlabfv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gwkttxuaj.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gjuxkxisz.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gyhbgxqnh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gcrbeqldx.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gwntqpcie.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gfqnmhthw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gnujgizlh.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gpwumdslz.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/giasdzeth.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gwugmbopp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gqvgiprpb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/glfekjnqi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ggqmymgmi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gppuvigvo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gezobjamr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gltozoygl.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gayeausej.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gmvhktwzz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gainmqzjr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gwiqxvwxe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gscdixdec.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gdjzgmvvg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gnidsoxqr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gqkskqxpe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gkawmzomr.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gbhzkksdk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/grwufxvzy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gtkmdiiyi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/guhiuoyrs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gcqsbkree.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gkmxrfyox.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gxyjkzhaq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gdwvdjcfg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gmfomtahz.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gsdoodhrv.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gxhigplri.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/ggixezber.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gmyboelbb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gnbydkidq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gdvasafcs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gkhqrnwne.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gkhatglhe.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gbliscxci.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gmkohqlkm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/grtuyoman.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gpdisydgu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gagacqayz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gmldrppau.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gzaibkfzy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gkxxrsyah.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/glgubulcx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gzlifikov.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gnwnugtbd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gcietdjmh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gcxfaeqoq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghltmvgqt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gnkiwimam.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ghcxuhxxu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gjhevmvvx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gwisemxqz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gzikczluo.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/grrjtgrab.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gjuamufij.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/guxhercxv.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gkostkzcr.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gvzwlpqhf.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gphlomgfa.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gynuaegpd.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gkljgrhyk.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gzpeugoar.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gqkcxvafc.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/guufgjfxa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gsxkgkaoh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gtnffdybo.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/guzmvjyov.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glqwvuosr.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/glrdjtewu.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gjlyuigkc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gcsvsjdxy.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gvkpmxrnd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gbmltobls.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gfqxcfkti.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gtibjpabv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ggzuygsar.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/grzceybag.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gkxsdpcxx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gvpvdhzqj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gjziytcnu.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gufdgpygf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gztgnmkqb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gmpkhiigd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gidhwlyds.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gsosakfnc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/geqxzijcn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/glsqxfgsj.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gcywixtvi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gbztmuxeq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnsazdvue.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gvvlkgwws.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gevcwtvjv.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gtlcxqozs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gqivasxqo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/getgqjqyw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gdiwckfmj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/geiqeogse.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gojptbtxf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gkhhkuthp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghvxxdzcz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkfnjemwd.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gqfptemye.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gfispktmt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/glfrlqtmw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gblvtovjz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gsewhwhmb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/ggthsbdif.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gxbafoayc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gejhxqqbd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gpisjgwla.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gctkwrycs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/grjnybmiq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gxpwxlxqp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/giaoamtpu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gpdkkkcjz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gxcmpkcum.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gxzjnjrag.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/girlijsgb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gwdiasueg.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/ggvtlsipb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gcaxkoeob.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/ghlbeuuwb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gtnrqtpuo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gjjysygkz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gmwgsajio.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gxnntkfta.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gvkcqrxya.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gtnpmjeys.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/ggjqryhgh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gqznqjbfi.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gldqgsksl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghgeipuhz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpanqojdh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gyauwqtwo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gtztsgdtg.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdnbjdlpl.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/geshqrlbs.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gmlgkigdi.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcqkqphcp.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnzijltmo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdxkgrgtv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggtjvxolz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gjmzxmrfs.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/giudkboqw.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsecxzekz.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfmhyjcju.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gkueeqzay.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gfksxggiu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gemokydhz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gtmzqbdeo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/ghjobmjes.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gizewiqyp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gvtobjxhj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/ghycoapnl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gieapnaez.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gkzvkrecx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/grrxoskfn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gisrtgzmm.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/giwyoydhl.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gaicufkvt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/goetwxvht.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gchzeevym.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/glsyuvzal.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gdgvbvnzp.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gifpvsobu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkphkllwu.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gopbisbjo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gztlagwzk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gtvrvpwdu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/grlszwoph.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gjcmbffca.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggyqmkqvd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gifldftiz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gadgrjgzt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gphuzofet.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gwlrhwrnd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grzftdnya.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gudaojoje.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gatkiowxb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmrouufjj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdhcgbjun.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsuhuvdrl.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gmhwidusr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gtimxwcem.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/goykenarx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gqtoxdkdh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gatwhlzgb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gamvdrypx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gierzzlvf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/glfcnlqkk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gpwdhfjoq.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gylucvqcu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gjuginnlb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gsmlvhrkz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/griekbavk.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gegqdxqwd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gwdgcelea.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gnxrubvgz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gjelmrnow.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gzyudpfsg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfbadkavj.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gzjnfpezy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpzbzpecb.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/glophlnby.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gxzuwmnjv.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gclojguba.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gwvxtchpl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/geafckxzu.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gsboistkv.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gvosbppjt.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gnmbzlybh.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gkfikifco.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gfqtqtxrr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gntlmqged.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gkiyextvg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlojbwuh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gzlztyjiy.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gormhigso.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghrxuqvtt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gxxspkfwe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gwzbbspsn.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gcydybxol.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gthrxsczd.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gznpamhyk.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gaddckgox.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gjzqouvky.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gaqaysklm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gmwnogfcx.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gbdcgivyf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gjncsubor.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/grskmeafs.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gphouaxdj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gnmhuteey.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gsftaxgrl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/guolsavlr.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gowvsnqqs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gnsxlluui.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gzmldmcdx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gmdcljlsf.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gskhrowbl.sHtML


<!-- 参考信息 -->