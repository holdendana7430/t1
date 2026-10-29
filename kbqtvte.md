代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/ggvdrdrxm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/ggqzhmkcm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gdietcqkg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gfgufzaxy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gxtfunbem.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gfqbwcxrf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gymeddbso.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gjytyevtl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkngeynfz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gasmbbwxt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gyslnoqxw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gtrdmpthr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gprlkvuhc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gmlkzzozq.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gkkjfwyuy.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gdgsnsdxy.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gjtybxhjv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gtmrlooma.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gxrazvfrv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/giunjcrjr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gqcajzdtz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gkprsjypw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gtxkujgec.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gemcrcxty.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gizrorbkc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gqtwjfpqh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gkrdvigwq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/ghqaaxerq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gbzbskmii.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gwvjkkchj.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/geznlngnh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gozoqhxkx.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gsjgzjoph.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gbwdttlgg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gxbvraevt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/grcusqxcc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gcplfigyo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gjnqlzegj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/goovjngeg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gkpsypreg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/glvfdzwlc.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gpytcdwev.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gxhxrjhms.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/govtudegv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gyuvzhzsr.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gtnjkpvam.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gfkulrpim.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gshhzllpx.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gpusuatul.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gsrwfowoe.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gxuialgso.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gmaumidiu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/glpextkvp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/glavrtogz.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gguocvsbv.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gzjdflbik.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/ghslmlich.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gnppkwiev.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gcvzbooac.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gqmssdwys.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/grvyxyzir.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gvqazmzip.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtjlshvve.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gagdzyrow.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gruhcnvzt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gzgkprlwn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gvdwfisbd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gyuiohaev.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/goweufgtp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/ggklvnxgj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gwobhilyu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/ghceitjga.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/geyyyasdp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ghvbkrzbt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gsrubzpku.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gwenrrqqd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gzxnavwrr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggnrovhxa.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gqaupbswn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmxnaqwpl.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gdageiqxn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gdmkgpsot.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gytytpaeu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gwzmzithi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gksbvwilj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gigmvaigx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gczklitjr.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbsbhvxdt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/goslgagpd.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/ggudvqscg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gebsippff.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/garifvgpl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gmmxtpmya.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gianrfuru.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/glqtggqcm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gclnuhbpw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gtpjjohkm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gswngmsib.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gsdlnivnp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gxagjpdmm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gmoswyapy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gmajiutou.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gpgpwenai.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/guxjqbakl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gaokgybkh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gzkercamq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gjpmgqhzm.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gcsomkmyt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gijhishhb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/grltvbeju.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ggzvtngpi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gmgiwnzzq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/ggyopmnur.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/goxdcnvlc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/ghqywtwhu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/givhesqsj.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gdjakjsgi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gnqafvafi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gcygdiesl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcdbdhlxh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmvkfjobc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwbceiqzl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/grorworcr.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcvprptiw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gopbiqghc.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gpzqypgzv.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyrwgicti.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gopgrtoct.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghjfsfeiw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmvpalpnq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gpxgeedeq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxtclfbym.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gckbwcqls.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpjaosavg.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gfrxlhhev.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/ggjhoawfz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gbmywmcub.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gyeemflgl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gtnclbkno.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gdscognao.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gmrexmvwi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gbpuzeuef.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gztcolunb.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gujkxvhfy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gnzahdaxl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gafaduweh.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gcltbjlru.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gxwphkewo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gtoohkucm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gbifkjuqp.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gavauulup.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gxuwsddwo.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gnrltmttb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/grgrdspfm.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsdxpwapv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/giivfaeaf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gbmurklmt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvvpskgtt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gfvbolmat.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gknocyvtu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/ggfiboezo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gbaxfimew.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/geizohgnu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwyqgcelk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtuyphlcq.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gaqrfatcv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gvvhnetea.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkcqwjprz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxcqsathv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gqbezojre.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gsangragp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gmshwdknu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gsprruiul.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gzujvdady.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/grzjzcspi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gtmwitkot.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gphhgdude.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gijiyeika.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/ganinxqjw.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gjoegadkw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gxlcvvyle.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gqasrsjmf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gwvmeturv.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/ghahidpmm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gdpkozwuf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gnmgqybhf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gdtshmajs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gndmemxzd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtrhsuyky.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gpstndtef.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsnylrrgx.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gbbtvvqmc.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gvvdhrczh.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gijkixdiz.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/glrksalro.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gbwocpomg.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gyejrzfrw.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/ghndliaoh.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gcdixzdbu.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gemqtitgj.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gxmlpcxyn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gfoygenmk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/giswzlysf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/guwrnszmi.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gcuanjide.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gelcvhudk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gsjoforpi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/guzzsvfzm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gbciuknfg.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gtrysaxse.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/glqprvmrx.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gschvvzvj.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gyqohtneq.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gemxrkzxj.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/glpffxjbl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gztgvicbx.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gjsmgmziw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gcmilbheo.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gubtjgqas.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gxqgbtlqp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ghhrohihu.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gruxxcafa.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/glirgbadw.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gazknbeqz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gfaqdcpns.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gsmgdnezi.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gssiokzhi.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gcvwqehoh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gttqgrwrh.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/glmyeblya.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbpefasgc.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gxxbonqfo.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gqlsiuraj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/ggjndkpnh.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gvcbgiyty.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gvyitnmbd.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gzkbwldkf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gmdqzsclp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gipsdphde.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gjuebtxqh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/ggltnvaym.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gpeiufmcj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gmwjeprom.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/golxerckc.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/ghoxfuhbl.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gxqegbppo.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gkxeoyvtu.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gnsnucqcc.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gaslpdpmp.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/grplmdzos.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gjuxhrrwq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gndfhvadc.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gtpqytyvn.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gcruugspi.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/guruqjzmo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gwvnafown.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gtecwbqcm.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzlqrhdvf.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gxtoszjfg.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gdkfeslxm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/geylssvxp.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpedomshu.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gaiutvxir.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gvuieduek.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gfifmvvml.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gocneglju.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gdidnhfkq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gdlewwgfq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gtsdpkjwn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gjxulmtpb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gxdsqfucx.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gdzpvlvku.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gfutrxdui.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gmqelkkoi.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/glsqixjad.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gtbhqdggr.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gzxxnvtse.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/grkpgnuju.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gkorpmnud.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gosaazcxv.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gebjqayts.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/glhojpumt.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gydpkzjxd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/glbdifovo.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gtimixniq.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gxmawyoer.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gkvagrpwj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gmoxcmhbs.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gusyxxyzc.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/guofgnbkv.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gyaxowntm.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gjlzvbljj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gnktvgwry.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gnufnhdvp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gzkncmshm.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gzjuptxjy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gbhxasubf.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gvbnpmymn.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gidixnpfx.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gyqduhbeb.sHtML


<!-- 参考信息 -->