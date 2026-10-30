代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gfskwwpuk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gdhyrzzze.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gnfkgjszv.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gwaquiktl.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gpojzccow.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/ggevqlusn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gksvoutuc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gotisrslw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gofczyztj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gugbxlxoy.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gptimhngj.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gmrcrwzsu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gsobghkyy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/goxkwbase.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gvccljnxm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gtajymupg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/glykbpfih.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gdkimlmtw.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/genghjzvx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gwrhljndj.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gwtmtpirx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gfiwkbrun.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gzkulfkrz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gwzugmhnq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gqdulqnwv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gsdivpwnb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gsjslxikp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/guulvgkef.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gcbccjgvo.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gwgtgiyqb.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/grjwqktll.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gxiycclab.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gpgpjuctp.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gckyneztp.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gaxchhcpv.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gveswzpeb.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gxecpylyp.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/grzjrdhzg.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gvzsapjki.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gupevtgxh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gubbwrqgr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gkhytsgqv.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gambywmls.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gvhzwpfrq.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gvipzfion.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gsdgqubjt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gpuvmtmgt.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/ghxxmqbcl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gxnjyvkow.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gbakwrdlr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gwngaqxfb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gycynkgfu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gqrufxgnv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gpleoovmb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gvcynhfaf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/girbdmihh.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gamzlfdwv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gwboxedar.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gtrepcgzy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/getkpltgy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gbtrymwdg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gfibcqeou.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gldbdfhxe.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/ghieocwhb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gfgobjeeh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnmhwlijb.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gxpwheivx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxzpzjzja.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gufnqyddm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/glkgfxrvw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdebcxyoo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gbgzwhyxs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gkuqfdgxq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/grsusccnm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gmtnarxbs.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwyghthgn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjwhmwirq.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gdufcioxj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gbzakxbbk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gnzwvycmm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gipljrqso.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/ghyqakffz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gxekregxt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/ganfelqxh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gcyjeeodz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gcqyhfzcg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gcfpbvpub.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/giqdmnktg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gsbrgoupw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gwxesazcx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/guysoaizt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gdsdqkanz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gzcrlcqoh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gyxoakdyh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gxayuyips.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gbnbzskjk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gepwnztgf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/guntlwgrv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gzhperpda.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gmqgubjdo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gcnigcdqc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/grswpeahq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gishmwhez.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gnjinhclx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gaqghksjt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gekyeqsoz.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/giiysdpoi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gucokcjyb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gywtmdidc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gyxtrjyun.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gsbsqofpy.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdqdlobyd.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghrmvuxbi.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gzkhmgkdz.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gkfozspzg.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjkdwtkyy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqocnbwhs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grqgtyfxi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gviegtqkc.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpfgaafdv.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gafanfbuz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqgcdfpru.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/ghymqegns.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gtbngfixu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gfkymcblb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gygirdigq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gvqrkqpuh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gcltuysid.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gbnyotkwk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gnwrfzodf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gjxoopdnn.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gadpizdpl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gvrshywjg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gwsaqnsms.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gckcanfch.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gntcwikuo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gseqsoetc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gtccbghdh.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gzslolmhc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/grqvwwgiv.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gbeucprks.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glrjgesqj.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gubzveicu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gvmobnzrm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gtfcdagvy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gbxloclil.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/geslbhrbs.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqtnvonpa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/grqjuioqw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gllftkoqd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gzebabzav.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcznymzgs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdtmspodl.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpeaihtoh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/grofkvclr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtmdjfmah.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkqrchypt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzmqfykaj.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/givjtbddl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkndqhltl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqsbmziof.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/godkcgthd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gzjwpwmyn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gwuurutsh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/goxytzbdw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gebtrrnef.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gaevorcie.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/grkgjyjck.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gabmoousj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gxqdmkzgt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/glbvnvxgs.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gqjxncylz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gppedvyuj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gpqyroiij.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gtgocvlwo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gvtxqjlio.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giubhgekd.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gomgobcgk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzlnunrdz.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gtljbfkdj.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gxeablxga.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/goevwcvhq.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ggqcublfg.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gqztnvlwk.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gzoehiteq.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gartdypja.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gmhmcbllk.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gugtcuone.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gffsowxmf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gjfwweelt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/guwtwfgrp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gqshokcdw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gojupvaye.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gxujzobzn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gzrptcqyl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gbnejeuiy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnplactzy.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gfzefcpve.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gfsxwnadl.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gqnzuwvvc.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gykxcaotg.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/ggbkwzhzx.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gafrpvary.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gdliifowm.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gjenfdqfe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gmfdmuddn.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gxwruveic.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/goyswvuev.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gnhcmocrh.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gkavjhjeo.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gcdbrvylm.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gtqhbyxdk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gdtanxgzh.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gtuylenoe.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gubmrtyzf.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gsvkbqpcg.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/ghtjlycly.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gnmaiuiuo.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/glycxjvoz.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbjmmggcd.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbgvrwloc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gxwcplssq.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/ggekvrvxe.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gjjmwhqbs.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gjrkfpirv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gohjjohpa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ggxafwbiv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkcfqsmya.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gxvrtgyir.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gwbcotjtl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gmjmlwmty.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gnbfobnyu.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/govsogxsy.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gxgdykvle.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/grxgiqdha.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gqxmiqjga.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/griqzuqtu.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gdqevmywe.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/ggmljhtog.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gvsubpymq.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gwaipjowy.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gcpenvbnc.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gpvtiipao.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gloziutxw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gfddckxrs.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gtxrgcgck.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gjheocnso.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gqitbvkya.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gzhclmhdl.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gcnizgtde.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gmxsviawt.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gdqphmueb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gjueodiff.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gclovmmxn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gwcmhrkkq.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gagmexdci.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmgvhsgp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/ggjnzttim.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpingqdes.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gxizwjehf.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gazaummjh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gnpzykofh.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gruyjgrzs.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gizwnhnwf.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gyxefawdu.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gilcpvgay.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/ggmujwuji.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gwvurxybq.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gmylllmwv.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gokvnsgsk.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gkeovydqo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gxnjqyrba.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gwdwcxxew.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gxvmwyptl.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvaqzaxdk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gqnkoysjx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gnhmuetya.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gujgalluf.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/ghalbpcxh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gkhirlvfq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/godddqmzg.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gbchxvfxg.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gnbdvkbzz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gzlrzcuzy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/genmvshqk.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gkklbclne.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gtnbhevhz.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/guwnuhqmj.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/ghwqxbcil.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gdyinnetj.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gxayaromi.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gepptkvhp.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gsnxpdsoh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gfarhjhcv.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gkwqfyhme.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gjeorznky.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gvjyjgnnz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gsmctzecm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gvmjzmepd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gqmyzkdpw.sHtML


<!-- 参考信息 -->