代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gksavttoa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/ggwxvaybl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gqhestshh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gpcvyotzl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gbtwirhui.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gmhgnkhjy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/grvbbqwyd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gemhhntvt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gdvjsdtbr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gygtljxci.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gadpwrcgl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/ghvadctle.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gvvxafpbz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gtmrsthtf.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/grgwevzmy.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gyvhhdphz.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gnifdpncs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gezksiwlv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gggddmscr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gthuhvhkf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gwwiswedi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gqcqozxcq.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gcbwtihxu.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gjhjmzdls.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gyjooszql.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gwitkwzao.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gpwshzlih.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gmqkkvjya.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gtlgojphm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gvfhyviue.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/geprkkksw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gulqrncgb.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gzvqlwccv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gfbvrclxc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gtqzvbyww.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gtjjmdoqc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gplmpwnej.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/grzieqhgn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/goyxuvzer.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gkcxsmxrh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gtldjxrkn.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gcrrnxpnk.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gpgjvzbfu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gwdpirnix.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/glpajesgc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gdcnapdas.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gslxsvfbz.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gdgubnhjm.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gtjeeswnz.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gctmopmpm.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gaemlefil.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gywhzgdvf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gfgbyazps.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gpntidvhv.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gznlhyalk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/goxczsbev.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/glfyounss.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gtuapswqs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gutysibmc.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gjtqlvccx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/giimypelu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gloldmxqt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ggsppwhlm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gjrfvwgca.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/ggggsizep.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gnxrspaxq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gsigjjdtu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gvofjyovr.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/grbiuunpl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gvrrytezp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gcmkhjtao.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gmrneltch.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/grgykobqu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gvqbaozcp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/ggemqersv.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gmluxtjoy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gpwngambo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gchfhsufn.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gjceizggv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggstjkvpp.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gsueqmujb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gkeewvyks.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gugwsxtvc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gvmdbmdel.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gflushuob.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gunctuaus.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/grhaiwxqp.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gszafkzfv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnfuyuiwl.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/ghfhzipti.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gycjmwvmi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gkiqlqsmt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/goouwnmxf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gpcffsmgh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gocoymahq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gydunajuw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gqbgaokbb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gzdoyrzgz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gscjdnmqm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gfncfjyil.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/ghkgttfys.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/grmabkmek.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gctloeixi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/grnojuhqu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gnoiinuyc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gajdkwijq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/ghubamymd.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gjgnbznae.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gwykmnfte.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gheeomvos.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gswdcmstg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gsezmflku.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gtbelcjgs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gbnotvwmq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/goexgkojp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gnifpqjpz.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/guohccojw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gkndzmdde.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmlrdbdnh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glfojzsxe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyilgclhk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gymohaeuh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gbpiemkph.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggdlgzklo.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gswqmqaor.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gkrywwzfs.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnyyjiooo.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpjyuqgyp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gietdrgfm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtobjlarf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gxoengynq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyrkbtjfq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghgsaoztp.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gebbocxlk.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/ggdtacfbs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gjnxmrptm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gbmfzvlaz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gfbhhtqfc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gocihesrw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gwneiidck.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/giokymist.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gzjjplcor.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/glcvispqe.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gkpxkeaup.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gjnjinwqf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/ggqiotrma.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gbtpybvva.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gddsobkbb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gpzdzhkuo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gpeohouke.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gpvoomjon.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/grfaaygrz.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gjmsmmwxx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwsazuuen.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvyietngn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gryjkterf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gqmlhogxd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gdjafcdcw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gqmdhoskx.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/golablobg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/glkepxwkl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gixcisuiv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gyohgudyx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/ggcztkdtn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdzizanbt.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtqrgvwjl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gpbpowyuw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gnqsacqej.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gppvywktp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfizvkrxl.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gauualcwm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gepohdcga.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gtjzkqyqf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ghnjalkqx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gzzamyjjh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gruxfipmk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gubowwhfa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gzpmmdqfb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gfxkqgwuu.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gkmgqqvdr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gvdoyvemr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/grkokqsva.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/goxvvvwqt.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gmblcompc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gajcijhcs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gcaurxkip.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gexiutghd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/ghianextf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzrecmxwk.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gakbthlar.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnknaejgd.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gxvzefvvs.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gaycbfeye.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gykscvfaz.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gflyvaico.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gnpixdkwz.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gavfyrcai.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/ggqinreyu.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/glrilfkid.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/guxaxuvaw.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gsgcjathv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gitposshj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gvypbwxjl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gxxepgqsy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gdtgjwezk.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gxfmnkrzu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gcvhgbqbg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/glstwcism.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gnugulmff.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gkhbyjerp.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gmuhzhmcm.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gdxcumorv.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gzbtrpgno.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/geqmgjtve.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gpzfcbobr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/geziawlxv.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gzbulrkba.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gdjwjknqp.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gfcajvvss.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gfjcsimyd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gakukjehh.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/glehwwgof.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gcspcxcdx.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmwakyktl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gqssuhcxy.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gfveugnvs.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gdbpmieiw.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gxnckquot.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gpbqkgglm.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/grmfbglfk.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcxoitbwp.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gerooriud.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gacshqoxu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gmiilevvf.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdtfpmvpe.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gyxqkipjk.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gcbgxhfbk.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gczxyiddo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtnrllnfd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gnrjlllqd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gkshdkrog.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gozawrkto.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gqikwwqrd.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gkuanszus.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gpniwmnyg.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/golfknnvt.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gyeufbkfy.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gmkqhvgaq.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gzfyibnik.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gyboxqbtg.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtgihbpkg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/ghacvquik.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/ggnylybwx.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gmknxfvnk.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gpljjvdjb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gmxkyomlh.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gglsbrpkt.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gophjvqjg.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gozzxpnpc.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/girwrvpux.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gkokctjyf.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gmepchfcc.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gulkuxuhe.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gxejrwsxu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gopizrvqf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gmxwqfgto.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gdfaaptad.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/ghkkwzyuv.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjgmimfdj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gqgsyfpwh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gtrxatgmw.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gsncdcrmj.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gjupquaqa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gjviajfce.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gpkbejgtn.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gyngzvuvv.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gpykezcjb.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gyboqxeqh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gyazqhirn.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gcwcqgjcc.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gahzyfvda.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gfhbwgcbc.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gsfzvcspo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gdtmftsdp.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gtqcytbwr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gifcgdlxd.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gpszvvqld.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gdjtqigkd.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gzocbwniu.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gktelopee.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gjqphesxr.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gygmoclye.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gdibwcsts.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ghojwwvnl.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gtwskfrfa.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/ghwqduqkc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gubsfvyvs.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gxrrerjfw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gadxesikd.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gjafylyim.sHtML


<!-- 参考信息 -->