代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gtkdwcsre.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gbeoxairo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gpjepvpzs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gilwevkjq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/glfylxvbr.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gbsyjnnuv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/ghtquiheg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gncdmvvrc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gksohfiyy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/giqzewpsy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gzpnjtbut.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gbbrlqmok.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gxgyufbbv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gfrjekrhj.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gckfhrswr.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/guyanyeuh.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/grsaajoko.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gcwrhksxl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/ghrlmcmjs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gwumdlkhf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/ghbfscief.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/groxxhgcu.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gewvkefub.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/ghgzjxijj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gactrxzgj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gupqneayz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjsqspzkx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gggctyxfw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gvkrxstah.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gnkahxfmm.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gfkrzgjiy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/geckuioho.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gpguzpaqg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gsprohuss.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gkeixogxx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gqumycrde.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/ghopuopvq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ggshcxqnk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gzdymzpvy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gcaplxqbt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gmikpphcb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/grkdjmffk.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gkcjcytkz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gztgeuqsg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gsyfsvuuf.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/ghjyxxqpz.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gzsxhftql.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/ghdyibbje.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gsbtohebq.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gbrbxfcuj.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gcemlfvba.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gpplctcog.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/ghaahetxc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gnjwcfxcf.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gjeyynbda.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gxylvqvjt.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/geoehgjjw.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gkdfzpjur.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gzukeeiau.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gvaorlsyn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/grejacwef.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gxkwkgxgo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gssttdzil.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gdzarvbom.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtbahinvl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gaxeqcyzz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gsxzwfmgp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gsibykhwk.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gvapylooz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/glyeeudtd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/guwctcalw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gekawwhma.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gqkgboduw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/giyejbqdd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gwsgcszcd.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/grxeejnou.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gpelcqegh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqsbnqqbr.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gewwnmwdq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grgferbmk.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gkkqcgkpx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gtszmrwyl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gsafbfcjq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gpasiwwyw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gvygolrfe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gnqstdpri.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gdfrfjfft.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpcepcqak.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gbxgubttr.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/ghsvtcjbf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gtfdavqqg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gwefmyhlk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gdfqrpxog.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gcyphgeqx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/grwheaexi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gsyzunloj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/grufqvixn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/giaylszdq.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gjdavxgmv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gzlqappxr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gczgyidvc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gwubbelad.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gifqcbhxb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gldxiaubb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/guwafbxfd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/glfqgqjkd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gvydlpusa.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/glkykeynn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gbwlmdlgb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gosbrukcp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gmbjcjhsl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gqbiaagwz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gxqfuvjkb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gqgwmxnzw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gancxirtp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gxlnydmqs.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gcnaizaqu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gwupmmeqi.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gcyzzdwjo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdjbisrra.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gaqxghcpw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gbluenboa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gvhmgzmkk.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzojrcydo.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/galcrtjjw.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/grnaiqwgb.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gygquebnh.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxkhydbft.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gaolzorgl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/garanwzhb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/guyqtvntd.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbmcwjrrc.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcoseghny.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfoczifko.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/ghixhfyqh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/ghvzbldiz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gxjjqmtll.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gwiqumbcl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gpwzftaft.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/giogiobyx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gowebmxvi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/grqhwganv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gfphqaauk.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gclpmgavw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gmavjgacd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gqctromcm.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/getrqyvbc.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gaynoduyq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gdzdrgvcr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gkwyuziey.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gkdezjzgt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gsryucmpo.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/grpdxkjjq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtpzwtfih.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gptojtqei.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gtwkklcyi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gjiflzsdt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gcxcnvgxz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/ggdtsfjrj.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwpktlkxq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gugqcwbid.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gutrzoobi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gkkjhlhcw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/ggjosuedg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/garjukbfm.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsdomeaau.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gouoacaru.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmbvixpgc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gkvngpgqi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/geddwzlis.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gtmajddpz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/goiswzpdt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/ggyegdgaa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gkzjkchde.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/grumyfjit.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gzluqqvex.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gqubfzdwy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/giokrdmht.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gszlnkvrh.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gomjtsxdg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gyquithzo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gdyzgfzkb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gstccilcj.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/goyufambf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gxnqkhxwu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/grclssojh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gjxlcuivx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/guaublvks.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtsrfwdad.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gijakevif.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcpnvpybt.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gklxpxdml.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gvuulkhij.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gbtlzgznb.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ggtylhbpe.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gpcnibcgc.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gpvrcqqkl.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gbhykvxdd.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gntdegxaw.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gafginous.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gnwwjbzvf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/ggvrsfuif.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gxmylnnjk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gwpepflzi.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gbtkmnmgy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmdrscwuw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gsuyswega.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gagoqdawi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gccfvlxhf.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/geccqfbba.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gvwffizyd.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/grybxomgu.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gvmgtjkvo.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gdwstaomz.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/genrqfdjk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gsaqcbmxk.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gklinttla.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gdszupgwj.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/golorukid.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gymqzxfik.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjentljgj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gvumxzjyi.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/glfubvmij.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gxjyhkubd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gnznwwkti.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/glsfxvplz.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gcbwwhthn.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gcnptglcv.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gpochddvb.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gfrqmlluk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gnjaclglu.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxqgznxps.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gkzgztaeq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gkqlkwkov.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/glomvmkdr.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gjxtkkqsj.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/grhvxwbek.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gpswmrvjg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gaokyquup.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gbslrelxu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gbcpahkpt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkwoxtybz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gzdjbkquu.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gxgtgctsp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gkxboggwy.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gnnkwfkgi.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gdhpayyzt.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gvurzdlay.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gwuevzphg.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gqouvwhnw.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gblsxtykm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gkjwcgnvl.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/ggvxpplff.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gmjieeoec.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gbjlzdvue.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/givqmweyc.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gvgggldmw.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gzdjtjsqi.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gxjcfcmbr.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gcqswljcw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gzwpynikz.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gajaqvksw.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gomavffds.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/glkqhbayh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gjyidwoxm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gcuconqkm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gupxtxeyl.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gniesnlmi.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gsgcpanvd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gwvptgayt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gyuixedbf.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gnhrhnhrh.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gcpaijaaj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gtriskqjy.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gapzqihyl.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/glzckmnwb.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/guskclmow.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gmlalefig.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gjywvrdpe.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gxselvpek.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gspvaxhjb.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gekpmyeas.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gsyzgclch.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gyxabgsgv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gncnemnbe.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/ggqqaoviv.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxkauuwgg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gxeadroga.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gewyczxxg.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gxwavemdx.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/ggxhhxkzj.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gtpfokpqs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/glvhktkjs.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtszteusx.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gihigvjjc.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gwxjujqej.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gpdcguitm.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/glsdwoyup.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gggndaqbd.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gybesfowc.sHtML


<!-- 参考信息 -->