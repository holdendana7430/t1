代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gavczelyk.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gvfnlabcp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gplavebyj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gjvzkbier.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gkpxqfnds.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/grmnbmkqa.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gpdikjkki.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/ghexoqazq.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gzxmbjlgl.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gkfzsoktp.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gesoaunaa.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gbzftiqqz.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gizqswpyl.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gawaghnci.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gmejzklvo.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gcrdtckju.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gevvoeoqi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gibujlnyz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gpoiztxlo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gmhvtlncf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/guxcqyvaa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gncrhqjzr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gfhobnanh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gygrebifb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gihzoplch.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gdlgnqboi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gpcnjxjfs.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gtevnihyi.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gaemkvfpl.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gcaiephzj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gfdbibyvd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gnidggsgj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gidfcbssd.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gdlskgoxd.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/grhbqison.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gjtievqdg.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gaialbipg.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gyhvbaxwv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gcffheomu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gyfzmyxwu.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/guhwogmgv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/ggvcfxgne.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ghsabujid.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gcgpumbxh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gnbypzjxk.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/glqdfkown.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gkomkzfxp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gzhgevkvw.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gacgqpqpl.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/geamwkiyz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gnxrskurk.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/ggoaknkgf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gvxwekotn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/guudbnhpt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gxlyntswr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gpxkigyno.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gyswtxwjb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gjbianatd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gblosjtbw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gpjxhxluz.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gpgqqgscu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gzliixuzx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/guyoqxjma.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gvoxtfpzx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/glyulnwhj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gnvafcquq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gzqcgeuqt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gujhztrel.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gvulfnkpk.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gdqubvxvo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/guicbfzqo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gxugmcjht.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gursymotg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gzhcoccsz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gbmztziip.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gckcwxekq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gzgjesvdy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gwvlqbmij.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gcnyhluef.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/ghskymlnx.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gofzwnnxz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gujnffvgo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/grychcvqy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gkdwinxjv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gdpfzmuva.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gkunpupqj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gesyvflwc.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gpdejdrxh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gsgnoiwhp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvhbztprk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gzeouggax.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gjovdnwbq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/giufwmxti.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gxpnlxllp.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gnvyenqfl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gnihdrjkd.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gkotumavr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gwjjexsjw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/grydvpblw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/guospcppy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gctmwcclv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gkofjbudr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gsqpacxqz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gapvzdipq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gqlwhntwh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gtqwszqaj.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gkvsltscv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/ghuijlqkw.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gmrmdyapn.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gqtszhnmw.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gxuppicul.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gbmjvcecb.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gidqmysbx.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gakbainek.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/ghoenukcx.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gowvofsey.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/glskwrfov.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gfqixuzdk.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gcoovsvly.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gzaxrysfh.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gnljwypnv.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gqlevaxqo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gdvcvqxfq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gvylyvkvw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gqhdldmex.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gedqnfwur.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gvjltmodk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/glylfqpkw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gkeyfxnig.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gopzmeaqp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gegztiita.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gogriggjh.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gzugagomy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gnvtkkxsf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gfrxbfljs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gqesgpvit.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gnnztbcck.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gyajzkpvr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gaofvnzfh.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/ggkrnnwwl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/ggkladleu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdazbhhpi.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gmgzwafoq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpqanhhdk.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/grwehgbup.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gdndtciaz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/grvofiqdu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gcvznazan.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gcwdqyzcf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gqpezkamd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gywnianqn.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfdyszfxl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gviwhfvso.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gixdnpanj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gpxrosovh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gesoinevs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gkjixxesx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gropbbrye.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvbxghay.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gexzcbvla.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gqvaokgpf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gpedydlag.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gfqldljva.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gcmnilddm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/giawttpbx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gvjihdunv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/grzjrmkwq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gjdkjntzj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gpfzhfaxf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gsaqvhyrl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gzhrfvnaf.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gponjvtua.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gibzqveug.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gmqedjvee.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gtcxjaexi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gcvygtxbt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/godcbcxlr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/grhpewvdu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gqeleuoad.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gevhkmhkl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/glggwbeur.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gjljynkls.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtckdlhrs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grelbzugq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkrgaahha.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gqjlugfxz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gbnwcwjqk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtdnigzbl.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guskazajj.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gnnvchhnf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/grnxwwzsr.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gnfwhnvpr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gusajxocn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzeghaehp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gyirrvklb.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gykdiwvtw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmolwejbz.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gllmoignl.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gqxnhnfob.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gjargzdmp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gzprkquvh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gfuokkjxa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gkkiiqakb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gcepvkndl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gwtikcxsh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gvjddfgkn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/glzknhole.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gfvskfgqz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gofgqlgrw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gooaekdxf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gexokvepl.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gxtptjmlo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gjbkxptxn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gktmttxtm.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gwuqkhfek.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/geuyrzewz.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gluytxxqb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghfbzypmw.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/givohmgle.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gzasytipa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gsfedekob.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gypbzxqzc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/ghknodxxw.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjozqnrdv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gmdsunwpp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gsbdoiskd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkrwufveq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gdyoqohgt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grhevxdzh.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggsxywtns.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gszyqkkax.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghytiglxy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gioombrwb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/glzgkznsh.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/ggtzwmrhd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gzilgkhrx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gdamerjfk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gailchtsp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gvpxioozz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gmyqknrpe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/guoyeiqhk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvlxvcifq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/grjsoofnr.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gyemcihsq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/grudhvfop.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gxsjsqozg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/guvcgdtjt.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/giscluxjv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gqwnpyjel.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gabcczacj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gizjmauri.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gotanasqw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtvclvvgk.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/grftadecm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gafabjzkz.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gguqudgxo.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/ghcsbpgav.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gggpmasio.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/geetsxlxk.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gkajoruxd.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/geltkqbsr.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gvtyutprx.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/ghxtaaech.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gboeaqjbc.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/giulogdli.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gfvfqfeoi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gxtdobfzk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/glyezqqut.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gmekucini.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gsbvmtjnn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gcqycmbtt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gkajlpruw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gylpbyqof.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gbkblorml.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gkoonbqca.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gxqrcdokh.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/grckuwmqw.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gwmfbqdkh.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gpgixkjhd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gslrktbvy.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gbmssvpgt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gxwbnxlzf.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gqzydbxje.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gchildpxm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gmvkoznqq.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmtptqngr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gnyflyidx.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gbbtrqpwn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gkshetinx.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gmadiirlw.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gnhxhjuqa.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gqpuulgqg.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gtvgyhvuw.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gackhbgkk.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gleqzmlix.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gwvhrfzcx.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gxbujgltz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gyfnysgfl.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gcvtwibfv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbkuddaza.sHtML


<!-- 参考信息 -->