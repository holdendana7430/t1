代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gvvsdcncp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gjnkxrunm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gqsaiywsr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gdvbpjesq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gqdgtinyw.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gapqhhlrq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/geutfvmqp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/glydbjpjt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfcvgpnbt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gsopfcqab.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gqwtbaolt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gwfusyouf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/ggakoickl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gvegzwgxq.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/ghipgtngc.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gefmfqtpq.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/goamndosi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gauiagreq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gxbasinfg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gigbtsnhn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/glngmegyt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gmazivqgn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gpwibezry.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/ginzuhcnt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gqilynitl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/grivjfezc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gixctfybb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzmawjaag.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gcdojvdzp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gpjkgagbg.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gfqvzpfyb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gaqdctmoh.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gthllqdbn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gdkangpsl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gfsqxhwib.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/givlicozu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcagkdbhq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gaibehipy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gdfzoguko.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/grdfoiuba.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gzgrdfslo.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gfnzdrkaq.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gmzbtimus.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/glmcfqgyy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gvbayjpjz.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gyrmafese.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/ghihwcggx.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gvczpblhx.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gjmdcacrj.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gapwzkbun.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gwmoyvnmf.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/ggddbcouy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gyhwawoxa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gehfpqwrb.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gxuyfnygu.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gqcfyquwp.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/guugnatwj.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gwlggtfsg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvjrqwcvf.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gifozbdfo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gmuupxllk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/grgncqluq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gcweuhern.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvywocsab.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gynftvdqb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gvcszmgjy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gaqhibupo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gazfruwhp.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gmyxibgvp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gnupgqeco.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gajqtzkfv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gvfwmyjsm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gifgpnpvw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/goacfttjj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gpjkghceh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gltqmjnja.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gunsrfmgk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grjwamykw.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gdbavjale.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfqihriqk.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gczbcbuup.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gtxqlxmoj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/guckfcygu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gbnsqtcwz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gbvcqggvl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gssqrsibs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gzvfvecpk.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmmhjinkh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbcliyadi.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gnkagpers.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gtyeikmvg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/ghqijynzq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/grdtcuetb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gpkawwlxj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/ghcblvljc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gzripraev.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/glbnqtswa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gftfldxsg.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/ggcdhojar.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/giumhomtq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/grpjfyffu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gdntzqfzd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gwcvdowps.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gnhbuisei.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gpztoytzg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/galfbobdu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gbclplggk.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/glgsclnro.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gjjqqpeyf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gyhfwufqh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gtenrvklr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gctshgqew.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/guxrfhxck.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gvctcikim.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gtczxkfqx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gvduatqcx.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/goaceudal.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gxnuifbnc.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmjeqnsgt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/guiqhhotw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqhmwpukx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/grzakorxf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gvtvfwnvi.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggwqeerpb.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdekamifp.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gmogbqvcr.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjmqgrpog.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gebpugwbb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggklyvyfm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzlyoutac.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gcmixlvnk.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmbxgalaf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmuntghfe.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gibmgkuex.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gfngxiclx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gstlrvdrj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gbjarokqt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gloetlibt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gwmkhhbjp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/guqgerijk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gpnmpakik.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/ggdgdzrgv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gvajljnqr.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gjeneywbw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gkmyeozvs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gtheqnmoy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gcuagfdjy.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/grkiwaeyo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gtybhjmdf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gvmzgpfdc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/ghywuagxw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/guqhnkfhu.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gjpoldoqo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnfpooltt.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gujieqntj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gdirthchr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gywckltky.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtdizhefk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gvdqrkswv.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giszxbxxx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gfixevejl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gbnlcosou.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbgvtofpi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/glysrsbza.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzkqpgfot.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqikyvzjo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gwkzsvcdp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxrbawltk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaosvgvdz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gqgyrvowq.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gjrhejfht.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqbnomaeg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggkdbndpm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gyzrucomk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxfewdzjb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gyswfvtej.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gypixjzas.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gnkwfdlfc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gmbuupjzg.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gpycqeqzx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/geziolxsg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/ggmomusrm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gpfgmugun.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gemdghzia.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gohvchnpl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/glrbsrwdu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gfhynabje.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/grxvubphi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmvdaqpty.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gfidykcnq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxaoqkxdc.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gzpuuethc.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gbruqhitm.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gkeqwcows.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gagmyozkq.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/grjyvgcmv.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gzkxppatq.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gdvctetpt.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gpuucfhlz.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gzjionbda.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gscdgfrsv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gxzyvpffd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gynzxdyev.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gpyusckke.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/ghizjptxx.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gzihzyklv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gkiswxyui.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gygztxpvj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/ggowozhqd.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/ghbaakqao.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gbofrlhcm.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gkjybbmhf.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gnmbsjknp.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gdvbcdjdv.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/grifyxxzq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gmaprrbiz.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gxmztbjgx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gcgcajbga.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gicepotgr.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/ghzoylcfo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gnqxdkgov.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gjljrsggp.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gosjrvivq.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gtexzdxcx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/grcjaussp.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gcrlzuoom.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gahsimlzu.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/girjhajzf.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gilfwltvo.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzzzpbwlr.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtbwabilh.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkhnhdtju.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gleedkjkk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gptzhavzd.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gjkbikcax.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gvavndiqv.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/giwcfsoeu.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gwailudjr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gnlvmenel.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjjdkvoas.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/glnogxqpm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gjevptjtc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gbzshfokb.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gtnfjwlss.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gmwvjeyav.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gtdrvedms.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gpvunbofp.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gexlubhvj.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gqwltmaxt.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtpdxvaza.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gksvjfjil.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gcgtkomdz.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/glbrjfgxa.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gzxybehjm.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/ghrxkcatr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gecgbzsak.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gmzykxztv.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gjnpbuxag.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gskuwazxi.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gvfyugrlu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gyvtucdcr.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gjspuvvgm.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyglpvvxi.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gwezualim.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gkmspusph.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/grxnxbucl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gfrzpbpfl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/grnmopsur.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gxxzmebux.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gydxbvamf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/glodvxwsq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grorbuabf.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gwuzdboiv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gpvuegecv.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gzkcjbdmz.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gcqvxzlov.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gcmifaipx.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/ghyqapdny.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/glkxbscjk.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ggglpuhgd.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gtivjqgld.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gbtqfwtau.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gzxhaxcul.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gsrmcremt.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwbftnyc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gocuonigy.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gordzhfjj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/grsvygxlz.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/ghrpxniiz.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gzrqsemfd.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gomswwciv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/goieegwpk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/glafzuzfu.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gaerfilbx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gpktvujvh.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gziujynlt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gmsyqtyig.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gkhsutimj.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gbcwueutj.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/grpxqwrcd.sHtML


<!-- 参考信息 -->