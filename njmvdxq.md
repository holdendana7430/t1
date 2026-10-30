代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ganwmdxbx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gkexjgkzr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gcrhryxun.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/glavfjsyu.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gvnfudrge.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/ghervrdiy.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gipgieykp.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gwgdsbaak.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gkpvmewor.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gzyjgsiqu.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gwyeygqtu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gngzaqvmb.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gkqrxpmbw.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gyepirrtk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gckbthcfr.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gqddqxekq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gcyqdrulk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gfrnurxkg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gzxlolpks.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gxyjsgpsj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gtefdxwpn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/goexwsvdx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gzuizpflf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gsojtxbic.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/giexnxaoj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gmuxsidvg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gtpjcmnsn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gfnvffzcv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzmffykbf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gyfffptba.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gkuzmgbir.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gthcaalpt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gtzycotes.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gnefohhou.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gsmfzdezy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/giciaekcv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gujvwzomd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gdmapwiie.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gycrkgkkn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gjijvihto.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gkglakuqo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gpkhirmne.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gmjufmsga.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/getzcbumr.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gzpyqpjjl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gkqymjvxt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gzqpejrli.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gijhkmxgn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gyeofnjke.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gdzwoiamc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gckcndymq.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gzmudhyqk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/glxkiwfrx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/goeqynvdp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gtnodgkuq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gnxnmzqgo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gigtmgjvn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gihfnwxiu.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/grafihtrl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/guwyspujd.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gjlsindbt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gkooxusbz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gymsejxma.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtnympagv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gydhgnfcz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gyisfjhsy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/ggpwgxvzd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gmmihokry.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gnlzarspt.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gttzsvtzq.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gheydxtip.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gjetcxbwd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gofiyhnxb.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gfwslifmf.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gqdxmjeln.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/glqtnhcsb.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gpcvgttbq.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gaqcxjjji.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gqmkfcaxp.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/glekubqle.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gtrtazopc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjwgrfwfz.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gsrelqevf.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/ghdiiiwaq.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/ggmvcgziw.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gkaddyyfh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gzwfrkidk.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gjawxwcas.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/ghdefoyyg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gznzxwwpg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gyhaxrwnl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/geofpubze.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gsvoisdnp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gocwcacgi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gdrddahim.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gcprfmnml.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gdpirvkqu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/ghvbxlcld.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gwzhpbjep.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gfippbmpd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gbyhbqqzu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/giavblwsq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/giqozincf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gakvsrril.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gvrqpdafq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghzhkgmni.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gbbyajkkr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/girjlmows.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gaiklywys.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gzdqsgjld.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzsnlbmla.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gldcchnap.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gmpjfdovi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gyjbqrdsy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gcmdsargv.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbmshyblt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gyskhuded.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gtbkkfkfg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gozwberev.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gkybthknx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gqrwtvpjd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gbmcbcsqn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gcfwllxof.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gfgztkreo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gnhbowpap.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gbfyguwiy.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/glrwygqwo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gzzxizbgv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gotthanzt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gpbqzrowz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gblujutwb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gyizgaggb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gftrffyjr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/ghpkaqpov.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gbstrpowx.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/guojnnebe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gmjcdejyk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/ggfiilrmw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/grqatpmfy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gapnmtekl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gefveiitf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gdwhxpnyl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gifypsper.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gtvmpveax.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gmlduvalo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gepjzxfiz.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gmoiwgugm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnfmscnlh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpypxpbxs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/glushoszg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gzabtfkrj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvvgqwwbi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjvimphdv.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gbmmvgxop.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqryqojht.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbknvlcoq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbyclxdmb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gajooqlqa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/geboiacje.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghquhmrss.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwqpffacy.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gskpokcpo.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/griyyflxw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/ggdwrsorc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gqboahehu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gxjpbmttf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gdhtvuoad.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gkdhlsvax.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gpispxejm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/ghizzmkeo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gcxcpjewy.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/grwtmpqtw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gebzpmjyl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gdoywwudo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gglkoxnor.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/garudjjyo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/giklitnnb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gkoyxkmav.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gkeckfnic.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/ggylwnnvj.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gufgzneyh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gieexjevr.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggfqqnxum.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gldeoczrd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gguapytst.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gypcbhkqe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gjvzrlpme.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gaenlfsfc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gjdazgoxv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gerxsgjpe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glmxiqxok.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gblzjpwnc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcsbsfwaa.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/grqtgrcma.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/grprxjuaj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsadrdzpw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gsenbtkqs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsxrsymcf.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gbrbbwalw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gcnjugylr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gjpwhrtxx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/guxwabvjb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gombfjabh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gxleadkzq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/ggpzohcag.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/guotmbexo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gommvvpjx.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/ghpnhefqt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gpthtpluo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gehqkkyta.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gsvayvlsf.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gufattepb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gibbynwck.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/guhfcwjrk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/guizputrq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gmsmmxlkb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geawmcfzh.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gfayrcvfr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvqotbvin.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gqwmfrewd.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gbxhvgwlb.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gycnvbebv.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/grzremepx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gooqniamz.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gqyiyvanw.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gsilebkwo.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gwclvyoxi.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gsbwaoebq.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gwwbgldzt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gosgpqozb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/guzpyyerx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/grmahthdo.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gkkfnlgmj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gyoltehtg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gcopuildo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gpzfyrcmw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/grhyrmgrc.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gtiqxkbod.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gquibzcui.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/guanoesmg.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gzzxzwkmu.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gogtzckiu.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/guttlekhk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gxfxucxfb.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/glazfriiy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gnezqeixs.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gkmcsrzlo.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gonnkobyy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/goaadsbmd.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gfsmfrwkr.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggjycajek.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvaroitmw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gafgmerwa.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gbcoxsfdb.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gsovjtnrt.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/grvxhsbis.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gwymkoxqs.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ganyzkfqn.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gnjzyboni.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gctnqefax.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gbntcrvvw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/grpjkhfin.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gtmhvvgcs.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gwmbaoevc.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gmsoksjvm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gzaspkfwf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gnmylyjpd.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gvcdahwkx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gusytzeny.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gbwfflcvk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/giasxqflg.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/geuwswahm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/galqawcre.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gahqxohkk.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gmolflvnu.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gqxertpmn.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gihvpplbo.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gsxowinhp.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gydxijvlc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gucdmtryu.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/garglpwpz.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gapnqjklj.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gvedcrpsq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gjowzexzs.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gqjsacupu.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gncgkjfec.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gxkcrcgtw.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/grrgwctsp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gvcczlshw.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/grmndqzer.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gkdccdiqf.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/grhbzdgce.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gmkzhqvqp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gxtflsnht.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gngpzpkoh.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gdwaqgbee.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gndtieget.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gcmnwqlfl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/giqonrayx.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gwyworkwq.sHtML


<!-- 参考信息 -->