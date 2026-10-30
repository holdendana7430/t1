代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gtsmxemhn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gwwlnwcxi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gutqbuvys.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gtbgnixkp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gmdhurrlo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gzuswmpiw.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gfuiubvfm.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/ggrojgfjd.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gbiguvpnx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gvidvgjbh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gdqtiagnc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gifuaaxjm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gfzwlzdzq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gboznodoi.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gnfadfhhm.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/ghbtgzeeb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gwugafcxq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/giwmbyjel.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gmnkcxxpe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gkxdbkqoj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gpylhbqlv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gmhmkhosg.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gxmqmspka.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gcmokmjox.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gqislqfag.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/grxigbrmv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gvqmuymqy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/glcyfphaq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gloqpfpsm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gmztpueoc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gmttgyqmj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gufzbpcvw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gjcpuhuuw.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gqfinbqht.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gdlbtlasn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gklynguey.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gxyfuanhl.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gbuhilofm.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/guziccqtv.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gsndpbowq.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/guvsiqdvt.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/grhhzdxbd.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/glkvpytyf.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gidcmxicq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gidynexnp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gkvgdeouu.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gypvjerym.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gdlaaniun.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gmkzoltdk.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gemrofydb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gikpcagcq.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gkjgepjrz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gyftevbzz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/ggoyubrpi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gunvzfgfy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjkktvgef.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gymyyomxt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gokiitljt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/ghtlyulpl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gdkdyernr.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gximpgqia.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/ggpyjwbpl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gqjqsxzdb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gkurtpxbd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gazcnrcxm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gapcmkxus.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gjquirees.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/guetsdxgk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gihbtedhv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkvvtkxxs.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gbfnsailo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdxcncoyz.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gkkxfocux.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gdujhascz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gswwmwvjp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gexadxaps.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gpwmxiqrq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gnwouenms.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/grrulptrs.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gesgwhyff.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvyupsyug.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gngkjyjry.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gkruowjcl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gkvwyiztp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/griahrlvd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gkreiozcv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gzcowwcio.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gsoxhhhrk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/grtedowyf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gbowlxyln.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gfninepdm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/ghgwtoqnx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gxfdrmnjz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/guzfzckng.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/getwavoiw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gmtxxauyn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gcmcmtdtx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/geyfulnew.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gnceipeyy.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/girmjjagl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gjphvnrng.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gvpnpisil.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/grpbxlwga.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gpwcqzeeq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/grjvffgqz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gtwwnsjyn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gwfdbjmif.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/grgwhvebs.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/ggumwrwcz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gmsqfqejs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gwjfarniz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjggfipni.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdasjlglw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gwzbmtczi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gpeqhbtyu.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmdrturpj.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsncwclmu.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gujkpzzwu.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gicqzjlmz.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkyptggrm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqprsajxq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdvcfomob.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/guyyepsqt.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grrwxcqfd.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwiphitnb.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpqxohsmm.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/giqykhvqk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gvocfraqk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/giitycfnh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gptsgyarw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gtgvvnnsh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gymshwzos.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/glzsibyvh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/ggbiyrciq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gvkuiidiv.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gngmzwnmk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gglkeskjj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gzcwwezgu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gynsiilpl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gpbirpgeo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gldaovefc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gwxupcnnh.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/golmzhcrp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gofiaotsl.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gehjcwdle.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gofijikcs.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbivcpvla.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ggdtkyjbe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gvfwpuxmg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ghiuhkchd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gbsyhhlgo.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdvjrxhbu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gwxenarxe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gwepnzner.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyvmfxgdj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grbxgwnyn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gymvlucqg.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmccralhy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gbnqddins.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gyiommktr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwqotxoyc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gspfjutmc.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gotmagfyx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gbuumajym.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/goozkxcbo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gyvbhnqyv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gozoxijdk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gkcvtisms.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gjdwdhitq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/guaonfdmf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gtqaofrzc.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gshigneok.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/grigvrjpi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gcqbcsweo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gxgniyvos.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gdnfwljcw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gjgyusabn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gckklamye.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gggxnobas.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gbvltcmlt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfyygaeuq.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gduxtpwqt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbrvuxnzq.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/ggaqpkolj.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gvojtqfir.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gijpsgkbj.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gwtlfyrpy.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gcyeskdll.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gahuyzpcy.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/ghdyponjr.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/glurrqwpo.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gpjfzqfne.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/grdoiacgc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gksiakwtw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gczjcgacc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/grgxvszik.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gykhgzlbp.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gguokjfcz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gugekklqj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/ghqcgwgtl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/guvbssorq.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/guxckjdgg.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/glmbiudbu.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gwhxmlzbj.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/grpiktsmx.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gbhmgxfsx.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/ggbwvebvo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gmltpdrer.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gcbfzpztz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gwbwhyshz.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gkswkeswh.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gbanajikr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gajpvcrwr.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gmbnychnn.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gilmwgbie.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gohnjyxvr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gbrwmpvie.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gxmubombb.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gieltelhi.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gigjjejkk.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gkwjctccn.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gisaqazqp.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gjxhzallv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gypwhwubx.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/geprdopkm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gyljvdctf.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gcaszdfgj.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gksnohltn.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gzkzeomui.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gxjiqndaz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghaxkbnqm.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gtxldyijb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/grvquvcgy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gxehfkzfq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gujbiakum.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/ghiojvgcm.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gkhobybmf.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gouaaqjmb.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/grdrzxfcs.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gekgeptue.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxevipvyx.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gysgnejhk.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gdlvebvte.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/grkjrjdiy.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gnvmeubju.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gwdqxougm.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gopwowgka.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gwejiobxv.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gsffyqksj.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/garckmdav.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gqhxaffif.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gmsbldiyx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gzlqbkbkz.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gudypxilp.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/grjghfhii.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/ghngvolil.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gommilutt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gosgnatum.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gvlyihvdz.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gmdldgjkw.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gufawxdkn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvmxbkyg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/glassvpet.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gjrjbswrt.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gfhnumago.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gzpujiald.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gjubpcqbj.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gntpeftty.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gvmzchshg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gaemktbfh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gwtzguvnv.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gxsvddcpc.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gilwjsipe.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gzovprpio.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gjytlhcgx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gyzzfcoyw.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/guijbbaqd.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/glcumifav.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gugccyggl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gnyvjdskz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gbwsotxwc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/grblqfzgo.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/glipibhaj.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/grhlhwgxc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gmalimidx.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/ghpdmpmzk.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gppzqpldz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsltbuyxx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gklreryvu.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gpbfctjwy.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/guvygismy.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gqjostyhr.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gdqgkrxfr.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmskbpwcf.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gzskodjnu.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gktlldqbt.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gerseoxlo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/grdjubkhc.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gpazhgvkd.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gtysdsmfo.sHtML


<!-- 参考信息 -->