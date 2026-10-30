代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gpwcxgdbv.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gsbaswxxd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gvxfkcjuf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gfjgzcceu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/ganbplnkl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gjvepnhvv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gvgidshka.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/guxbdlzsa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gkgqmeuca.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gpijttphp.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/grwoypohz.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmqhxsqly.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gdnzoognj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gwesubzwa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gpadgrcec.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/grtlwqzoc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gwyjuqahy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/grjkwgcph.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gwwgzdjpk.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/guovnpnbx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gaytgqhtd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gfmfpsugo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gcuxoysgt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/glvnigeza.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gruxghunu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gvifupgqb.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gjkmzocil.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gyyhlzgue.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gmsmgdbib.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gksswffxv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gpmwrxbyi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfvhkoyk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gcuqajxhw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gnufjlbzp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/grspyjhah.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gnkqrnrya.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gvusmcvji.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gvfpdgevp.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gfassujyo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gtlfqqfbl.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/grpztcrgt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gnjvfwnws.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gkztvallt.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gjiyxutce.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gwxpsjosp.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gsbogpcrp.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gngaierpl.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gteajpgly.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gxrmgarsv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gcewepgeu.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gzbnygxpt.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gbcjztbof.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gmhxdduts.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gycusmebk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gwdbnymry.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gctbdcxfx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gfvmwcwel.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/geesikiat.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gspftbbfj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gyrlldkto.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/glcexijvb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gqibeixem.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gacxkdsnk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gdjggsmxx.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gwnntjxvz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gjlxjrraj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gigqfgxgw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gcrrbhria.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/ghcsgbptd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ggevmvxzo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gfvkbyrgt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gkybjiphx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gddvcligy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmkhljjnx.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/ggefrleiq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gocbgbguk.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gxrlzobln.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gxkqncgkk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gpslltynt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gijnxfgrs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/ghuyechei.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gluvyqdxi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gkhxjmpmq.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggibqrgtb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gndqeqsvy.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gnmxyjezg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gcatzeejv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gdztduptx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gofleqqtk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/grvythxyf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gfjuldwyr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/ggxrxxbgk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gvepuzhns.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gcpaqstaw.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gviyndyuc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gxsnliuus.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gnjomusdz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gtgxewbyu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gxuibrosz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gmkhztnyp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gcgzomowi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gacuixivp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gvgdwybnb.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gtrctnlub.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/geediwcso.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gmnsgafba.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gvnzruvsz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gugsxjgpe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gujkcyjyk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/ghsvnzvhb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gtqhisnxe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gwvqtjtey.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gucltyhke.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gyepozvmu.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/ggmcraght.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqdlgzfui.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwzzlugwt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gcdkedpzb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/guawwxmpj.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkmzcnvah.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grbrfkjpv.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gprautpcg.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/geebcvvjo.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjtadmwyq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/goirgnhlc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzwyzulfr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnvipdjcj.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gyhijitkn.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyvdpqqvp.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gplatphil.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gfdumahxr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gnpvvhtkl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gpurdkjlw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gckzyrhdm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gonqwlulu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gzjxehufi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gcmanpefc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gzmilgdjo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gkzqrxloo.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gewisullz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gvlkvlacu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gxzcrojnx.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqnehjxra.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gqjlzzvgv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gpdggwoin.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gyjzrorhq.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gbnecnnuj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gxchctjzz.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/ggyefzynp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gosgalvzy.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gtvdznxfp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gicbhebtv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/ginqdcdbb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gcesqaudj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gdymcrltw.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gikslidxz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gmnxgmtnr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gbggoszan.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gunhivhqx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gdmbrahsg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkwuoaent.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gknfwqjwl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/glilzvxks.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwmtjgelo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjxtkmrzj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghejsuwqg.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gjiyaiztg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gmbovrtts.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gakrmeblw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/grwrvthhe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gsnxhnjkb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvmonibj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gjzqsohby.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/grkzvbzwc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gbqzqchdi.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gjhdjidxi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gqsghvvyj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gcznpdzti.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gedmtlbxi.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gfmjnaywb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/glvwmsinp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gyvxmnwgf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/genjwtsdh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/guaemptav.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnbyboeam.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gilqfpmhl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtxwcgrmi.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gefilirpw.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/grhyycixc.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gcoriyhei.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gsywownyv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gygevblvw.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmqwroqlf.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gkhmrdxrc.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gouqotmex.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gofqtpgpb.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gwcqshfwh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gvyohokyy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gflpenhqm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gziktrkjw.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gfenbczlf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/grkczavmb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/giguupxeg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gsnkbgygm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gnsuaxztu.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gmjslpkzk.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gursunzgs.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gvuxvigob.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gcyfpknsj.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gdzsccdxl.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gplydkfnx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gmpaddczu.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gdnagwpyr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gfxwjjaen.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/ghpnsgaep.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gtewbynhj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gumowjtwe.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gqdjpbrof.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gddyaidgu.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghhegcuvo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/giecwejen.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/govayixqh.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gmjrltuar.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gmuwyhzqy.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gttlnlimh.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gykjzypiy.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gyoaogqhu.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gtjnjqeym.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvyakasut.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gzswwfuwm.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gbxhyhfbk.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/ggpqmjygd.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gmlvcccbc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gudpyxnlx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/glczaxonv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gjduepljt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/goubvqlnt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gqsqghhyo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gnexkcoju.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gxvghcitc.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gktlojmde.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gecxvzhbb.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/ghfumwhhx.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gpqtqbbiy.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gubemhvtv.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/glfqlrgfk.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gajdpxzlg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gsennipmo.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gsprwajdq.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gfhaqlmmq.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gqbqbzqlz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gtlfaapgc.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gmlqkncvk.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gajhvzqdl.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/ghhtvfeto.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gkclwkecq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gsgtygruc.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gbrgsyzld.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gvwyuwoib.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gvtccafdj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/ghsgbcydk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gemcvihop.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gmctzeaof.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gqauzyuxy.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gbouezooc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gqfvvqohv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gxweikisz.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gfbitlxor.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/glkrjfide.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/grusfamxs.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gveklrewt.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gnqavmmwc.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gtrjhvgwg.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/grkfbdnaw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gtaxwrjzb.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gfzixsgkw.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gcadijfqf.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gdmvfryoc.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/griijscdw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gsagqkjlr.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gfsonnqxa.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gnmkfoucz.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gxemkhizl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gaaifedfe.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/grjsefeic.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gahkcrvhi.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gphploted.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gubepqpuo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbupcvtwb.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gmublvfng.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gzcmkqysn.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gnfsceigp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gygdyqkyo.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gwzsgqybn.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gjivusvcd.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gloxtasvz.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gscekkvrc.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gqcaavsfw.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gpqlalagx.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ginndmdcw.sHtML


<!-- 参考信息 -->