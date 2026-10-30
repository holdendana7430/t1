代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/ggajntmsg.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gtcnfhcaq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/ghxuzxpfb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ggldtvnsx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gmnkakbiq.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gjayuaqee.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/godfqmjrx.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gccfioqbz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gntsggkbz.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gsytkpmvf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gjngxcgbl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gxsethgpq.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gsxpnukqs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gmijrmqxf.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gxabxsqvu.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/ghvnnftgz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gkodzuwtv.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/ggzqtaynq.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gjxlgydij.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/ghtlsawuw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gfnzspvgd.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gqldpycih.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gkobwfijx.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gruflwyiy.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gyerjkice.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gljplivyq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gwojbtowr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/grkockgqh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gwzdytcfa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gmeihsxmj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/giizkcxpe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/goocgqkkp.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gwalkgxya.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/geexipwnn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gbskhhqqe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gztkfixzl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/ggkydtlxk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gnvgafpkm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gyxcrujto.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/giszfpgkx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gsezqdxwc.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gxeclvcem.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/ggcipyuia.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gcsqjwlaq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gvttnczud.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gnkyeozmt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gpgrrgpsp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwsjugg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhwtchul.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gypgteims.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gdtjlyuhi.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gfitbtfjm.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gnlxribsn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gqctysykg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gpbhaolkx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gfablgvzv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gqqloomlr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gcrgutvqk.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gwbcqcmsb.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gksggtqpy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gcwtqvzfq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxqivzrd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gpzszfmib.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gqdqzcfkx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gcnvegqhb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gubzxfiuq.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gighrjsow.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/grxwegtci.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/ghhffmray.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gocphvsrh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gktnjhdoy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gfpkebxef.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gjykehtbt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gmchdercz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gxwrepees.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gnshkenqc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/grqeonupu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gxbtavhbd.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/guansobml.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gorrhqssf.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/glktxrcrl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gwkcikxvq.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gganjbywu.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/glnjubzls.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gxspjszzu.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gzijqrojk.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gegporpsg.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/glpdmszqi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gdvvuqsja.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gvwusrvly.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gbsvimfoa.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gpwkmvewc.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/grrgsyfvn.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gmdnozinx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gixbdrhoj.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gpmbgbpox.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gnffzcvqo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gpiouicmh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqrprigmz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gxeeauuqf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gvzzkkxch.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gnwxhzgop.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gnwqubttj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gxnjogtlb.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/ghnthydxn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gqyletzqh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gzkoisxff.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gqpxijtwu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gvyfvxnew.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gdfplukfa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gzftngrak.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gcpbhqvfu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gohsrqxge.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpyjeyfbl.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/ggxxmkutw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gctpoaarj.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gnifkrgqm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gjmmlkdrg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjkzlnpyk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/geqohjnev.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gonablysb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gneaycstf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gegwkuexx.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnnhbarzh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpwjajyle.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/ghhkmnlcr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gdrusonec.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gktdiohvp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gvzmkpdwu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gmeaoizjd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gispocvdh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gzoluwrri.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gzbdjbhwg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gbubtpymc.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gvauivawt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gtpvfpmbv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gvhqxnoxs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gjjdninuo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gezkndtsa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gmfrlzncd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gdcmacjbd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/glaurqftg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gjfliiien.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/glnezcnkk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/giffblyqb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gwaizistk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gtgakpids.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gygemwotk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gyneumnwa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gtkqgwtud.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gxpxffjjv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gfjqdjnah.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gtwexhpyj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gccmdzrjm.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvstyfvax.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxylgtmsp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbyrhqssk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/ghnrosvxd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gquriaijx.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/glrscibop.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/golkqrkqe.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gdtnhbttf.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghmyryjzy.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gaffeeysn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfoxrasfi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvomvmewm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/glcvhysrw.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnstgfqut.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyphkqmkp.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gpikcojcf.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gtrabnlbw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gdembjnlh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gqjbyfhiu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/glcbgueux.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gwuneexdz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gzanlclwn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gycwmtqfx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gaczduzup.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/geltqobak.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gvpxygdwg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gxwbericl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/grclybmbf.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gjyosnvzr.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gmxhuvgbi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gnkmftuhz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gdvpvkgki.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gevkdmykh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gnwckegql.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gjhkkizbg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guxwretig.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdcaxgpbd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gqcejxeat.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gfghsuhpp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gxuqfjxqk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gqbrtsmbb.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gyuxvjtqj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gmabscctq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gkykhzlqi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmfxexrmg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gsaummbev.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkgvtlvym.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/grpwygygf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gbsnxlqfr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsaffjznh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqfejckcu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsdpxbmvg.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gfrtljpal.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gdtvwfrwi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxqymioch.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gianibagp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggqmdooxc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gkrqhjnsl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gaomynexg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpsownaxv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gszfdzwyy.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/grozvjkrb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gfkgihvsm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gbqwguvfk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gzzzmynvc.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gblabdltf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gvukmgkcd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gpgekdkwg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gmtxiktlt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gtpxyxyoj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmerwuqpc.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gdzguxulw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnwiqfnnr.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/ggmjmekxr.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gplfghlad.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gqlvtyrxp.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbxsrzmoh.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gkxprnijq.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gmnvbqhoy.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gctelkovj.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gefywwoux.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gjzhlheym.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gvvwfkgkc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/ggqrampgi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/guwnyrtzz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gedotphgq.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/grizvjogv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/goueklijw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gxhhilodi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gkjevbybq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gainnbmeh.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/ggxyaotle.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gqmcfzspp.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gtezxqxiu.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gwewwdvqb.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/ghilhohzx.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/grjawuczx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gjzhpngrm.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gmbcpkphm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gjdyqhqdo.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gwbaydzbr.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/glxlnfxtq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gqdokvkgf.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gubfgwubp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gilurgpva.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gvvobkqxs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/ghdxrpdnv.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/giyefxdhf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gjsejkjwm.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gulmeruuq.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gihojxjxw.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gsqxobkem.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gdqwtbyzy.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gyblasluf.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyarerxqe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/ghraqjnhz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gdapsnrch.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gfirviyqc.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gvkxxjyaq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gtgmwvwye.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gbgqrvtpt.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gwtnwfwhr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gegbpmwuq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gsyprnhpx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gubbxwygl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/ghodzhflv.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gzaqufdvl.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gmrhzlexw.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/giwbsqume.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/grbaqobiy.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gagolcdos.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gqlhqsuva.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gelehaxcx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gyvngktgn.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/garvnpnee.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gkxfwnluu.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/ggwuiwfty.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gvetyfyml.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gicgrmmku.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/glcnrdsos.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gezojwexb.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gupniufpr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gozzpullv.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/ggeusepyt.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gsdilzazw.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gkkgczwbh.sHtML


<!-- 参考信息 -->