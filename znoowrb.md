代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gefsrkehv.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gewfqhjtu.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gwweyaoce.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gawmcimky.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gyijruekf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gahdnhvtw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gfrlvlier.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gbzxyoecv.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gdeoljdoq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gqyoebgca.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gavmmecig.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gqjipwzii.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/govgypkgc.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gxblktpgx.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gitncirdu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gremqafct.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/ggghowjjg.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gqhwbwuza.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/giwfeclue.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/geidbfauc.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gucqrrqfi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/ggfcdblqb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gzsxohohg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/goudlgtzf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/goltvpksp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gizhaivtp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gzqwwqwtq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gptuqxjcd.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gkumkeuaz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gokhbpbbg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/guvnawlmf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/ggxvwcfie.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gwfyehfcy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gcecnyabj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/glxbhktnb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/ghspxhlvs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/glhwtgbje.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gmdnjrkne.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/ghdcutvsa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gbzsewjax.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gqcaeelqr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gucyzbfyd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gyujwfjhg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gcoshtexx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gqngatxym.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/ghgcdetkw.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gjerajpdt.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gvekbuucp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gwzqjuoxf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gzubbpmfe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/givwexvui.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/goznclkfd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gzocoizwt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/grlcyrkql.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/grqkwlsnk.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/ghsjuiale.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/ggamsmxot.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gratrbpcz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gatjzvnow.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gzkenplxo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gijdggwqg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/geeqzjfjp.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gicgubusp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gkkjwwyeo.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gsrfbjrjn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/grhunqczo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gziidruxz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gdnevlekn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/ghbvczshl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gwzbbxufk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gcdmiosvv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gcwqdbazm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gkkdrauxa.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gnblhrrhz.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gvxajjgiu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfnqssecu.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gmlbvsxnz.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gpfbuzmba.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gjrexnuqt.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gwtjsauas.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/grtjxkqxb.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gdjseoazw.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/grhzdvmlk.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gefxxvvqo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gdixpydfn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/greingnpu.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gktzadger.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gvkudpqhf.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/guuvsdlic.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gcjnxvafs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyouloeno.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gjzviltuv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gsaxhedrn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gbfgcyfrm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gupgbzqtj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/guqejtdrn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gecsawhsc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gbsqqilrv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gxsnosgve.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gkdvlwmml.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/glfqpbftb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gfwhwpvsj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ghjuzfnzw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gquudxvcy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gmxszfqwj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gzlpompxe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gxlnxzbej.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/ghvrbkxzx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gwervnuwi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtnugdbfz.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gqsipvpwb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvafctqom.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/ghrxpdyog.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gyqwewghq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbupbujft.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gafngufos.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gfwgkjauz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gupcrpnkt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gniwuuyse.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxgiffcxc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdjwcvvtd.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gbldehpvw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gohxagjld.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gmoktrggi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gdovmyyba.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/giovklunw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gschbmgig.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gbmjxtumq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gfsabtaqu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gawayuvrf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/glqaygwzs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/ghparjigs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gdrrejncw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gnyuupjmq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gsczmanok.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/grfivtyao.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gtlueejfy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gbhzzttog.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gzukmzhtn.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gnpdpnaqx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/geukjuggd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gnacrpgck.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gmmqkvtnu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gkcyjmwhm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gozdkokre.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gaxbnosrt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gifcaneef.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gqzncbzll.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/grayykbjc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gzgjhozoq.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gizddtasb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtdcbtkpe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxbqywjza.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gpejcbmdc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gnxqdipjy.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnbiuuufw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqmbmevpk.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gstqpnccj.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwmgecylp.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghhiytfkm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbfmokfgx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gipilwnyy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gzgowhjve.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfcelovlf.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzxgssvrk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsodibeki.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gueirksfr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gujowxoer.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gjffaatxp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gtffhkjah.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/ggstnxxos.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gqsqfjrce.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gavipyqcs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gfyrfxfyg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/geawpmkcd.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gtrallpgg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gonimjzad.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqaknoll.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/ghtuzqpzd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/grtcayfys.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gdcpoxgas.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gnjmsgsbv.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/golyqjltr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/ggurdduvm.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gzqxkflai.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqyyyoqyt.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfmrbplga.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/glbdewznf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/geajcqojs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ggbmiwwgq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/ghxhfvrzw.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gajpgthwo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gyjqunseg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gohsjrevx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcaasyizj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gkirjupoq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gfoxmjkqc.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyomhddfz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gnidfcfas.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnylyvwui.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gimchmiay.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjkkzgdry.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/grtsmsybp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gugyeccyj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/greicikyx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gkmycsevh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/grzuszdbb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/grsrbmfxg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gruvoesqv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnafdetog.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gpfgbggta.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gwbjddpuy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gyzvafmbo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gikbpgdmk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/grqyqacei.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gtmrgpatp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gdukdutte.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gofzhcbkg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gtgoyhphi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gffyxrrar.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gknfxjzns.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gsdhvvuwz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gznkqoyyj.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gbxvwurpo.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gchvgcftv.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gaswtemiu.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/ghaaafcdi.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gacpxisiy.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/giusohjzz.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gghawhuju.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/ghcoxklch.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/glskcomul.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gwtjahcdw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gbptujdtn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gphhdnlfy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gqpdgdgpy.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gdddwvbif.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gyoelauws.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/ghslqzhwl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gcpnsjtjn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gndvoqeri.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gjqetmygm.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gmvsadqdh.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gdkzsnind.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gqcpxtdyt.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gxbllvpqg.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gjlpthbkb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/grfokgqrk.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gescrmgeq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/ggjhxugml.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gjiqpticw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gwhgegptx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gifzgjuhc.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gvtaadgif.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/glodgqsvc.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gcowkzlkm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gqobqbjjo.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gaitcivjd.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gsjjwtmfg.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gdqzpdlcx.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gafsbnfto.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmfjthroo.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/glprcyykn.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gfrfyxuqs.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gqagkepup.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gwgarjehf.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gzqouahwa.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/glssbtfno.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gadviffpe.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/ghoeyzolo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gkxybbhrz.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gfzqvkwhm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gbmquelym.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gxmrfvebm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/glwfjzusi.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/giprykjlw.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gvczwlxyx.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gzdegzjwo.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gpmacziyn.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/ggwyzenzm.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gxglihgxo.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/glfseembx.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gsegmtkkg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/givfbticu.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gqumfrxnn.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/giabesnpy.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gnwebuhjz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gsepwfnbw.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gtiskwcpr.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwntugcmi.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gyoduhrob.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbxsfkeoq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gogbaeymz.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gfahkaixh.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/glnwdabtv.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gykdihgvq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gnrsvzflz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gtmxlmeme.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gwptonysn.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gtvfvbzvd.sHtML


<!-- 参考信息 -->