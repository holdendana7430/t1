代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gxjkwawov.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gyqfjdrhk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gfhltdyjx.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gqshfqykv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gqlnytkbq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gpfrgfujk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gyqbubjpw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdvkozoo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gqvliazam.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gfyqsnzlx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gbfouhpuz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/ghmuztfvx.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gkosuypwa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gdxizlgyv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gvwnseciq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/ggovpdmob.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gqwwpkein.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gvvfmdfgv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gkqjxjgdt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/ggwcofsrk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gjamzraym.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gdpnnwyyn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gnyuauuod.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gwlasmktu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gcyhrjmkq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gzcqpuvxy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gtkevwjsn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gfxdvlobo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gdlbywaup.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gdjvcmpzj.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gzhaiknxq.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gyrcujlia.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gvgnztquk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gyrnjcact.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/glnazovar.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/ggrbhidgw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gtapajpcx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/ggmcwoxlq.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gymvrrmnt.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gijyydrtb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gbzmpfpwu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/grdaanehz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/grhszcmpn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgezpcjp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gwiwzljyo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/grvnlmqsd.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gojqmbdib.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gpwezusfu.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gwglcpgvg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gkbihefcf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gqryezeya.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gminsxpcm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gobgocsgo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gsoqjiidf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gydbnicoa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gruhykezh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gnqwbndze.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gfgitbskp.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gfgstkviu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/glwvcvsyh.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gyraweodg.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gdvgbknrm.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gnxpqetrk.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/glvescbzm.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/geytyzjan.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/ggrvbiwws.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gkkfqsuzt.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gkzfkrpol.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gwibszvte.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gqldjkuxz.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gslwivebq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnbkjovhh.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/grazjkaut.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gzyqeylmi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gsembuoha.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gszgxxbry.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/ghgtdoiuf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gtdeqndhf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gkpfgeilp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/goydzjusa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gibarrbwo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gorwtgnvl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gbrmrdjym.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gtjzuqjer.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzvaaothf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gwksrkxen.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gmzsbasve.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gfmkelrkx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gzzsbeyqs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/glkjpcnmw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/golaypoqs.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gcjjeoffb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gzwturrpb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glepiphxt.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/girdprpci.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggdjmayoo.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gjveqwisb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gpmtpyrip.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggkonwjsp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gdxhelknj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gbwfkmkfq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/glmznljkh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gmcwpiezy.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gepsequxe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwwhlecao.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gxvknxrae.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gxhjqszav.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gglkboreb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gxxinlknz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gnjsnotgx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/ggnjodedg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gaeledqit.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gjyiiznxt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gysivdtqi.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/ghqxxncqs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/glwtnltnh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gwotuzkne.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gmgcdxhkf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gjbqedldk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gilaumlee.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gpoghndrc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gnrfxbiur.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gpgidrshl.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/geketodbb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gvfxzbpxd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/guvdwbuir.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gmztbsciv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/ggmckgini.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gmqjgpspj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/ghvmqnzwb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gnlinnkor.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gjyjvthpl.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gtzwmweqo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gbginfeim.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gphtqehaa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghbeechqg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbtececpr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gqgycudfc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gntirdexp.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/giddylumv.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvwdimlfk.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/ghkbiujsq.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdqgicqsf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gbuukhywp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gccgxvxim.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghdkvcnio.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gkdiybtyg.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gltjsjwxh.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyzdrmiwc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqjssddwr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/glhsyydut.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gflcjrrhv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gqwvjazuf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gvndadsze.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gqgzgwxqi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gzyvnwvox.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gfteqlktg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gthqfyktp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gjceumsfj.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gieexfion.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gohjbzrhc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gqjctiubo.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gabxrktxt.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gxjkisnkg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/glgyavoqb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gxoremrkj.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkcxpxeqf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gznckrzza.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gquxwtqjy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcilfdahr.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gymcyhwbk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/ggerebohy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gvwdbspps.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/goeqhbbpj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gtqnyqvua.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdigsjonl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gavbfyysb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gnvymyigb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gaezsrmxi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqujxpxxv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gocwawhdj.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpiezbild.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gtfzcmiji.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gufnmtlnb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghuaelpsu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggvsbagsc.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gtaftnfbe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gugwfwckz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzucgvwce.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzcxfrxwt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqqeipcbs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/giawntmxh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gestrngaf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjkcainga.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gkrmczixu.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gknpemxmp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/giwxzaxuy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/goadospvl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/guyurqnho.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gqqickywk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/grmckotwz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gvxjhbkas.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gnbwjiqfx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/guwysnjyv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqkzkncgy.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gcmyzwjvc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnkrjbnyz.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gkqaomdxu.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gdltbjmeh.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfisiloeb.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/glbmmxkuk.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gwcsfntyo.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gpitsdozy.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gvnicgpdk.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gyutyxfmp.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/goehogmea.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gojpxvmdn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gabdujrew.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gqxzkllfm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gmhtyzugc.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gowmkcgsf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gunzyilss.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gzncodqgg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/guiygrdtx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gffjzpgve.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gpbjylqxd.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gmjjxbgaw.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gfkbglzqr.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/guurvchev.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gupbwmpzv.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/glifrdegs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gqgsbmous.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/ghojcqsmn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gssnwzcvw.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gmreksttw.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/glkwnzofv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gdgracynr.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqreagdjr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gywfnjqac.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gvwgbkreb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ganampgcg.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gifustgvx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gsyrnnnyx.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gakhqmsyu.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/ghplnczql.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfbuhcufd.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gzdzadarq.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gobmohufq.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gsgntvkrm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gogdqndug.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gskujtknx.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gykccvwom.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gwfheqdyz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/grrwxitvy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gifkaapkw.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gsjmptqkj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gzgmgonzm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjgpvyzq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gahljxkeg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gaadqxsqn.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gtvtljbzo.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gdmsddmpk.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/ggkkxnsnr.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gkmawbtth.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gjfkcysic.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdgnhgrqv.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gepezsuvq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gquvvapdh.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gijmoyxft.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/guqutylmf.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/guybfofjw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gzbwfnigz.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gtypykqwl.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gkznnyved.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gokjgutff.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gxzlrulkv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/golxtvgxg.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gafwmsclw.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gxezpatnm.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gkeszcuql.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gqwwwawzu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gmrrlaooh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gslbflaeq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gqnnlkmmp.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gruxkzvcf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gsfwspnya.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/goqemkheq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gvcddmgqa.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gmrxtvcgk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gmkaeomxg.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gxcucprsa.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/glmtfhrfm.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gpvgwqgor.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gkigvzxxj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gpdwrsyeu.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/guiariiuc.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gnxsuewlt.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gwfnlcuze.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gqyfydtgh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gueugjnkp.sHtML


<!-- 参考信息 -->