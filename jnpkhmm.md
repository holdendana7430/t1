代发 wailian999

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gxyjwxlxe.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/grjuzmxpc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/givwpojzv.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gtsnaeiyg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gynbtbtmw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gstxobbvi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gxpvlijmz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gcvbsdlxe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/glwpkuitk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gjotnghlr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gnjkvzfns.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gzxmxlisw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gowpnudew.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gzxqlhics.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gstyputbi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gfomwpoqq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gxcquczxj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gtzblvdem.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gdhtbibhs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gtgnsgsjt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/ggdxxaghs.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gryfcbmuv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gxnxjaylh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gegojdhad.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gjvwhrqzb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gfyvyecox.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gowltzdkz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gcrfsjeci.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/guiplirku.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gdkzueovx.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gayigtzfd.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gneszlubj.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gnshtyknj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gcdziepic.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gxxzzlggx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gqkujwsqj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gijaolvgy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gshqxqcww.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gfgudkqkc.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gdngeiuck.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gqnwybdlh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gdiiqsimp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gbyekdmku.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/godmshbiu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gzgaliosd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gajfewnpr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gaqeyuxui.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gerlmxhww.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/godrffqea.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/glsnssoet.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gobxetbqb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gnxlafofc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gxxmvzbsi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gikkurzmu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfrjsub.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gzxcbinwk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/garkqtaxm.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gdtegypom.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gzikhzkdi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/glmfxqehh.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gnmqbugdq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/geszeegal.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/ggtqkkbmd.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gtbztslfm.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gkeioqsnr.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/giozrzbrw.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gofvgaxdo.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gtmfjrqgx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gbmbzsozq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/glddefips.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gjhjqjfro.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gqwosokjd.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gbrnlyssj.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gizeyzdqv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gnkploxsg.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/ggytbbvij.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gnukwswnh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gwvgoitts.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gwllwsgje.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwzvtstfj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gssgfkolb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gaqaoxbkh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gfroigxvy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gfnjsdmbf.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/giypafbiu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gckvfnykd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gplzgiudp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gpydebnjh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gqvzvpsyg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gypcypsdb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/ghpzpnekb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gjdcyqzvn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gbalvsgjj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpgspctlq.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gigmqgwsh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbeevwhtv.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gyzoooaez.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gyseenpcu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqrfwmbhj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gokauucjg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjjroxdgn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gskawjgzo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/guixmyfhb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gresitbpf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gujpfhspa.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/glqdvidew.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/galmmgzyx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gvosxwjfs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gylyqdevd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gcfkmnwio.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/goamiodex.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gdyqaweal.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gcrcorhep.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/genelxqip.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gnbkvirmi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/ginbqykam.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gxpeqktgv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/goaaomhfy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gtmgfrrgl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gyulkamqm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gcayqeilo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/grdbmktmk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gmdtuamiq.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gdkcthbjb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gxodbvmqv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gsvchnyab.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gyxnzxvhf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gooxrfmvl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gnpuxyrjk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/ghebgfiue.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gdfkwoomi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/goucjdwou.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gqupvaszw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gxubguyxp.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gfwpmkxti.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gthossiwq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gobdwlyke.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gsilocaja.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gprkrltte.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsqwamybv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gaaigznex.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/golhvlqta.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkplszhrp.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzybnnuma.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goapyylbs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqdogkiqh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gtcwebjtl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwbsloars.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goilmrrua.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbdrbeoup.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gqmbqxexw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gxqvccpyy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/ghlahnwkm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gpzgaveck.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gdspjmxnp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/glcppwdoo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gdglytnqw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gtmxpxhwe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/glwvfuhui.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gfhoqkrnt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gbdjejqgw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gyqqmztqy.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gvbbemqmu.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gnkqccssr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gsivadvjf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/ggecgvvzx.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqrzgaist.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gzttrbnav.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gjgqmlrap.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcpryqwbs.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/granxrvrq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/ggaeoszmz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/ghbmvcwok.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gunyntvyr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/goexahprs.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfdckjwen.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gmmfthbvu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/guitzlygc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkxntsymo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gamwfkrcw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grgeoejcr.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gajmmnzzh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gcceikwqo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqlmcunpd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grkycppji.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/glxhpjjoj.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gcraukqwv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gjkrmrjgv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gsxmjdaie.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gebsjgunq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gftqujstv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gvqagybcy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gfqcxgcmz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ggnsppskc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/glcikmicv.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gjutpphnh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gwquwrhju.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/guqwfaiyl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gbkmluhfj.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gmfzzbdgq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gxnrpkwqb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gtwwtzgei.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gwydxhewe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gwkqmrakd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glhgvmkpm.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gplxskciz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtttsleyt.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gnxrkjxhh.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/glynmiykq.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnpxiwlxw.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqxibijmc.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gbysxoomu.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/glrxxzots.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gdqnwojnl.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gnlnqqxhp.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gbrtrdure.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gmxobazzj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gasrnuzrn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gzqbsacjy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gsalzyyfm.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gcmeqvanz.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gytyepfjp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gxhroggnk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gpzngwvxi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gxytgdyev.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gbjkwylon.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gkegusrig.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gvyudkaun.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/ghslhufis.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gfapzupat.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gmkpecios.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gxzgkbino.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gbgjifvco.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gqokefgsv.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/geasxxlwy.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/glrbsbzyp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gwjgmkcfh.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gordwhkhz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbfeczvif.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/giylbeusb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gmwqbxzsi.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/guburnyfl.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gqjgkynve.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gakbmcbnq.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gntfgczkn.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gxmmrxtfd.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gdokwiwig.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqjuhmwlz.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/grfdcafce.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gbtpaqvvj.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gxiuvcblu.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gnisaetbo.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gotyzlohj.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gntazecgr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/glrrzstdb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gzkttjltc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gtutpdhjs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gqsabcmpp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/goeignfzo.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gzrrkwcqw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gelofopsk.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gflvrnexv.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gsmshupjw.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gisddlvdx.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/guvagpmvn.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gnyvvakrn.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gggktlywn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gblymjizk.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gfjjgrcdm.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gfuasnlvj.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gnfzbyzhs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gszwekcah.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/ggxggidwv.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gxdofrcbw.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcamboznq.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gjevuoade.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/ggckvvzwf.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gdosvpqxk.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gdyfhbdps.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gpfjqgbkc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gxrforzkt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/ggfaddrbi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gdzirthxz.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/guiuqghgx.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gamihliko.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gponpxdfr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gkyarzirb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gihspgagf.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gxafrhqad.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gsoniehzh.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gqakpvdmt.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gvojrfefh.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gtnngkyjn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gzenflyki.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gycctmtvx.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/giahfvqzg.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/getdklino.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gbyxiyitg.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gqtlkqcrr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gbwxwhqsg.sHtML


<!-- 参考信息 -->