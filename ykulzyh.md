代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gscpjngvw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/goqasvibq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/glixatbwn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gqnemuasa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gkpriwhog.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/goeejhttq.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gwvtytsgn.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gqqwqdycg.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gfyekipvo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gwaskqvnw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gjnkqsqab.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gpepubmty.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gcgwsanmc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gtrrkonvi.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/glnsmskch.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gdwxzlfpr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/ggrskfasl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gucoqibpe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gjonxgvyo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gqpjwglhh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gkupbpoas.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gwntdhnkw.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gpaetojfh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gyvsleobn.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gsdbfedbl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gchgzvhcg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gwzwvzenv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gfjkykuoi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gbswzwbnt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/guujwlnkm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/guiktxjao.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gtjwdegro.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gupdmmnjy.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gayrsyegj.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/grorovpcb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/ghzuqglsp.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gjsgicyxj.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/giknbbrpu.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gayhludmq.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gvpukrfav.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gyizbzvyg.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gdrqaxzcy.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gcwetkgqb.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gtriejfae.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/givmlssnw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gxvndocwp.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/goabrfnhy.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gkrnndosp.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gjvrqodxd.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gfgcokslh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gzmezyxsf.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gjpzkmkhp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gbjyerjjn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gixzdpaur.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghbmnqfjr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gvlwmqxzk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/glrppunhq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gqcmpkttj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grlwotvzw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gxadvmwyc.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gwrbaziez.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmqtwsjd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/glijlembg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gikiesdin.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/giutbjmef.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gibkqhvxw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gfrighrtz.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gbufdashk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gjubczzlt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghrmcfjbu.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gwoqitepj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gibrpxakz.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gzqbecrgw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gcvffdxoq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwmjwhfik.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gcwbnsdlr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/godwdxanv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ghpcqnvss.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gbqococtd.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/givbqpuzm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghivfciar.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gcwpsbcdi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/genkjxqee.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gisfesvar.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gqkfiprtf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gcsxrnndn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gkscyqklv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gzgqcdpwv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gvyyrsebn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gwpalrwng.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gipzpirat.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gzomqnmzj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gyukochvm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/godlfqled.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gpvktxzao.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gjpyyfxhj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gvdgzdstn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gwdaaymxw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/ghesxdqnk.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gzssmgsel.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/glwfefnib.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gsmvyzbte.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gueqkuepl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gnyfpujpt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gjowkshoz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gjhmugcrt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gskiwxewr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/glosnhpsx.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gagvbapok.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gwzssdzob.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjasfvmuw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ginjtbwfz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gophdekiq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gspmwxdnu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gvnrmkmcb.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdatttint.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsstdrgzn.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gnxkhtcer.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gygokejyf.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxfpmlush.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/giqsdyivz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwlwmftqf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gdtwuydax.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gaxnrzzfe.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjatliumn.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gdulggsye.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gtatnhwri.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gnxkjktzm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gacarjles.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gxqbdcrod.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gtqftnuno.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gmtjezjbs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gezqxxwrd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gjjnxsbkl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/ginwcrshh.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/grktpyhkj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gsgqgjqvk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/galhgsmfk.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gasfibzoi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/ggcpaepag.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/ghrsngdrg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gmlmyibcy.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/ghqesrkif.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/ganblyjqh.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/geharyyvg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzivyxnbn.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gaxlejgmk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/groruhdvg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gfjefpcqq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gtaliufse.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gejztkcgl.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqpofgktd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gvgqhvydk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gaglbqbuo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmjdvfarc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwmzbjvib.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gzackqvuy.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdchnpgmb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gvrbdleaq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/grggrowvm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gpuiuprbq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmdfxamya.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gszlhwort.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gtrzwifek.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gmhwqiryw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gamaeasyq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gygyqvlpo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/ghtgqkerg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gobqkzjge.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/geagmhrof.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gowgvbhmp.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gbqlfwefn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/glnjnybod.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gjgkynivx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/glbmilhhw.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/guoqnvawu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gjqqteuau.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gfwouiqxc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gydzojqic.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gjzsftgep.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gucifvhmy.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gpeispspo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggvskcoiu.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/grisuqpog.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/geujpbxii.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gaanhpnkr.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gagqpbszb.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gpaohjwhp.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbiqkbdev.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gopeuolhc.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gmwxmzzux.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gyttumbfc.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gcsukkxyf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gevrzjllu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gjgeokwul.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/glcqswlym.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gqtguvjia.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gdanaqdse.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gkeabssjp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gjjfxpjnl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gqtqetrhn.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gciorgoqf.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gmnygkiea.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gliclornt.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gahvcbgtj.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gvsmsohuj.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/groeoqjcu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gyamelouw.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gykgqshfj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gpfvvgscj.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/grsxgmwkg.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gybasainz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gmvdhoyej.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gyttlsfet.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gltvkjekc.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/geknpzxdz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gktriruwm.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gvoealvlp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gqylvlden.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gttlycxzk.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gljorixwi.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gnxfwcbde.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gysnnagoi.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gevkotrmz.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggqsdhiwp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gnesehyoe.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gbcxnhhyb.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gdsnnzqxs.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gbftouplh.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gsqgrdkvx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gvsbekwqt.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gsobwmrhj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gybnszjah.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbktdbqbu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gxiwbgcfp.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gaxcwxucl.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gssqkhnoj.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/goalgawhf.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gaifhbsdr.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/ggkfnnpsh.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gxdjotcsh.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gsruartfz.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfvfonrwx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gskdyfety.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gycdqrbry.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gzzkszqjv.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/geywvnuxf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/ggstjyfdi.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/ggldmszmw.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gqfzagips.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gifgblhgs.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gtrbwqnxt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/grzewmrbk.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gndhfeazm.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/glrxyhpjm.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gblnjtzfr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/glglpjdby.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/grzcqcyhp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/grzomhhks.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gwtfgwfct.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gwndxdgmp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gyrkjzveo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gxstwpwyk.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/ghcldglom.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gaxmagbsu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gcetfiowx.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gudfyprrb.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gsxcmsfgc.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gtbypkgpb.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gqontiykz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/guxmxzlib.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzzqejrrm.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gkbzlebjt.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gpfctavmj.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gmqskcjwd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnusktsxx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gtjktvqfo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjbhxtfit.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/giuscbndn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gqypwemrm.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gbjhwnuht.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gbjnacysr.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gdhauugrf.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gcbceigiy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/glnimlbof.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gmjtqicxp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ggmuuwwoa.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/ggcvfreop.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gkwazxipm.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gfbrixxvz.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gcexrpdyj.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/glsktwqju.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gkrzaprln.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gleakoclj.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gvdjekysw.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gjjtpqnio.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gaacbliuu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gdlcsjpkr.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gknfasxnw.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gosvmbfno.sHtML


<!-- 参考信息 -->