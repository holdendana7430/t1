代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gycxlwzqo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggmqwkxha.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gujjjlieu.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gjfzarywn.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gvosrouhu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gpjazechf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/ghwywaygi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/grmxwovnf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gpjfbzipn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gqirkmpot.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gfjvbjamw.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gtgglikqw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gyqpzyxcj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gxjsxrszo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gftvvyldw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gftgcczef.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gucjigmue.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gozrfsvgn.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/geaeeqmro.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/glaycnjyc.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gxspbrulp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gtdvrovjn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gjhbrxlfa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwaxvmbyw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gzmodcbne.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/glxfihami.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/glggxfmav.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gdxbvqmng.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/ghilawrig.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/grjgxnxpj.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/glbtywpzz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gktmiwoli.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gmsaihdbo.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gygfztrtz.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/guudftedw.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gaynqjviz.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gmbdrxypz.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gndlgqzqa.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gtsnifppl.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/getzgudem.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gtbuuaata.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gztlrvfck.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gvhegsffk.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gkybrjidb.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gnwfqufjg.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gvfwoksfs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gzulcqqrg.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gmwiwfyib.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gacndpdsu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/grstixwhn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/grvrojjme.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gmgivkpec.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gfkcpzdjd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gdxedrucl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/glkzxmhsd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gzwhrwepg.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gsxwcltjo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/giawpmynx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdlwidjru.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/grsxhqtcf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gimnrdtop.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gpawrcztd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/guynhfvrv.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/ggrgfptkp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gkywblvvb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxmwwhseu.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gxaigzrjw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfwfwpunk.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gozkesprl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gbxejqqtb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/grqpkskez.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gvzrwofiw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gpjujymsk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gydtnehiv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gjkrbqmjp.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyhtfytpa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gimzmfine.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gfncddbup.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/grirukomb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gypmbeeeo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/geskfdpxb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gafjsdmro.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gbxmakqbt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gzohmwska.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gloenuhuy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gzmkvcmwc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gmiefebcl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/grqrfuyqg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gbazalzca.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gqfinonpz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gbwoliwsk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gqvizupmu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gbfmbauro.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gmuzcacuo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gibqgzekx.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gvwghmwtj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gqymoycjt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gfnuigjjc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gpzneyziq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gbcrlwlpj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/grfulnikw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjrcvwlyu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gxlfoggfk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/grpkqsthw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gqkstadgz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gthzoqfdl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnmmlljxr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqieykvyl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwbzgxymr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gkqtvpbru.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gtvwryqld.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnsmixnsq.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvleqfbmh.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gifiaaxlu.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzkqamxvk.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gpwkukeha.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giltwpftg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqsrwsjgi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gsigxgczq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmhcigqny.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grolkkgdx.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gywhcqspt.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/glrxvyxpm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gizclerqe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gsrjkriad.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gemyznvdy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gifxlxvfb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gfsptttqk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gfqxvhubr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gghaaupsj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gpykfxemk.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gagyzfknw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gwkezemko.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/giraoonsq.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gpolupmen.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gbrwzeelj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gbhejoucy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gzfjjufkq.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gopliazlq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gtmulkzgy.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gbimkwisp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gofhhvreh.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmoqaswyr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/glbiihryh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gkuzmrcmx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gfwbcmllv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gbpbgdisq.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwqddogxh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gnorpiops.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gypssnjbs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grsmwpaag.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gwiyornht.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdfvxlykg.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggfwhodls.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gravmpnur.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdmwfornt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdpuwufeh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggbbioqro.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gznsccpfa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gshyqdbyk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbknbjltu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gajqbxddr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gskncdcbl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gaftszjrk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gsidatfpl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gtpbrdgjw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gnngnlndr.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gtchrpexz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gzzjpkxen.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gtrrtnxqe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gjhteknjz.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/goemwtoeu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gpokfszco.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gsklohzza.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/ggfstkwby.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gtfqwcxhp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guaaootgz.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gdiwtdcxh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcalqwbff.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gastbsszy.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gduaclgbq.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gyqbhrbjy.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gfycwncic.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gfvpxifjw.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/grujkzpjs.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gswvzrmez.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gqtuwpcek.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gkjsqrmcx.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/grrcnqouw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gnarfenzx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gjppovnba.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gjjdqfcqj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gnnkcsyag.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gvsvkwwfn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gdbspdlvr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gzcyltowg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/ggbvmvibe.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/glttjitag.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/ggjoiilyt.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gfmwvppyj.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/ginzzsvwn.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/grpxjzkjh.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gopomnfgl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gcjbbksqd.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gsouwixgo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/ghqanvwsm.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gsckmbszn.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gbjkkvhgw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfaqlfvaj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gyyoqowgf.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gjzgufdls.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gfvrsstsy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/giywkhczi.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/ghowakknm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/guqabslbm.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/ggfniknbz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gehuaqtyv.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/glymdnkym.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gkxozxpjh.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gnihujfuz.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gjriwdraj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gvjdccxky.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gcfwsyryi.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gcydqdfxo.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gijdrhewp.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gfnfrkkjd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gvatbkdqe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gukrmwyph.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gxgfgizby.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjsmaygpt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gljarpkrr.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/guuirjtyf.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gzygbylrs.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/ghkofksrr.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/ghefjqmjb.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gurncreza.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gamyptdhy.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gugifwcdl.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gtvfclsup.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gktxgskrd.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gdbwabeiv.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gjtsdyqsz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gazhauydx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gvdwgtmqj.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gzzjspcoh.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gepvjrxtx.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gaggoaymw.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gbvfrywus.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/ghzozhjnx.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gzzwvuwre.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gxfihtsog.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gswbhbzuu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gjhyclvrv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/ghlqbautq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gtdbzzsxs.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gqfuznrkg.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gjhzokvlh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/galhuualx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gnavhcqvd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gdfmzhixa.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gkmeypwno.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gcpzogbnm.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gpggllaru.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/guqsrqjpc.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gyzpbekcp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gobpivykm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gpzpnkyds.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gcxtnovnm.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gdvkixpsi.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gtrmavdvf.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gdsbjfwmn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gjwhqpqnk.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/glgmyjrfi.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gnevogbcl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gajyhusqq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gruhtfmgb.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/glykmxlnt.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/ghbzvzytb.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gkxbrnqlm.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gfroubima.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gayoxqnve.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwyossgfl.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gbjigqzut.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/glqgkbxto.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gggesuxoz.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/glntrhgni.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gbmjqbjmg.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gwhjmwvby.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gbeazwqpn.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/giiwjsero.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/graqnxuep.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gwdttxccc.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gwqpbyppf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gkoiuovyp.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/ggwgdxbgf.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gttfurenb.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gntkexakl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gssyziugz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gwbezicut.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gxmwroiez.sHtML


<!-- 参考信息 -->