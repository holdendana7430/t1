代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/ghlolzbcg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gtlfbtqqw.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gqeylmhqp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gesiemtrb.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gnzdjcqkw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gcnaggwap.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gfxeqkhjm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gpebmddqb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gssqhyidk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gzisvdwlp.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gflopvwzt.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gilnjwnsz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gjezmenlr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gvqjgeohq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gozyjmccb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gztclerte.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gsyubsoep.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gufcinhqp.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/ghmqnmfjd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gxuvmvlqn.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gclqaewow.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gebpxuhzd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gptrqsfab.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gshnriehk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ghimpihai.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gfammjpns.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gcujfqfyr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/ggqiycfem.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gpsfzrydd.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gbdrsubdp.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gvgjdzgeh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gmjfhntvb.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/ggjojebzp.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gzehknxzf.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gseqtbunw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gnoflcjmz.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gyxtabrdm.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gidrpokiq.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gxlhyochz.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/grpkdusvy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/grlwzrjvn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gpnkcyyzn.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gmxiewivo.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gfxlgwmnc.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/giwsfldzr.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gaffqjhnj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gpgtvtgfy.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gwuksxjum.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gmbndhfus.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gtpcvkime.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gihvqmnhg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gqhwqnnyq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gyptmtsbk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gfqsmnqum.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gqgvxweti.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ghxvetrjs.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gytbnvmro.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gggpptjec.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gfnmeyyba.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/ggnbvukla.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gmjbmpcgn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gitdgrwom.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gyuuntugo.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/glsvfiald.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gvztyznyv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gewggvige.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/ghwfkfprm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grgnppdrw.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gwbynsasy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gpngrggxf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gevstbxqs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gyvmmqkiq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ghwtaqytl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gybbmbodr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gqzbxqhet.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gipqhdfdj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxmfcxxme.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/glncdqwwy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gvqyioges.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gjshutuga.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gjsrwpnsy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gmafokedp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gmzhkhevr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/ggfcmftit.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gikohktqp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gxzajiyue.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/guhlextwc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gxccptana.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gjqukuxcl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gtzwhisyj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gutxngusr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gccslqyaa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gabshyedm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/ghlfwvtwe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gewmzqjkr.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gvoawigkc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/ggmcvpzne.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gbhxesjaq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gwwoorugk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gdpahtjwi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gahjpzbns.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gzricczco.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/glpccaiog.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gewyfqfwm.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gqttlwdqc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gugdwlgdm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/giuxnbgkg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqmyydsqw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghrxvnnzj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gsqixrgtv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gzfeykqop.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdamuurdl.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsxkkskqp.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/ghpchmhty.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvxaexgfn.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gzpjetrde.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpejokmob.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfkhrfbkq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ggorilpcr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnwwmyjtj.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdiafauch.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwoutxseo.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gxgrpluzz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gytuzacli.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gmbokzpmf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gzekcpuyo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gsbgjcnsk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gxcadeccw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gxniskymo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/glpsuejzo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gozgsagru.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gbvieseyf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gfrvvrdbr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gqqailqvr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/ghmlsbxvd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gkupuhdlr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/grqklfhla.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ghezixmor.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gyhboaiic.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gzoabbpik.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gxpqaoqaw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnvlkmrvi.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcupxhgkg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/glrmhzkjy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gmabgtbll.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gxjfnhzef.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gmrijmfgs.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/glwhukgmp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/ggupeamwh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gfyhclqvi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gwiqvafoa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gqktdcofp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guvaxsotr.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwukdvovk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gqzlayocz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guuzdyypm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjvwhbmqn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqwddazun.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gyeqvvqtf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gggzevtms.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gkbehnypx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gakipfruz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gqfeukehs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gpvbbjzbn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gwhetnlin.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gravnbntn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gwrmohwrz.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gyjnydntj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gsbostwfh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/glwrnpyos.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gpickcfoy.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gazmiqhuv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/grrvkzpyv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gukxbttuc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gsqcibmri.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gzowdgmym.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/golahgecl.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gunphbmjt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbfnagljj.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/ghryvqpog.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gzohnjyic.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gdhrorzcx.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gnunuvzhj.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/glceupxwo.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzboqxpeu.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gklolpupy.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gpsfdimvo.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gxtjazpci.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gexkyutbt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gexulabay.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gesrppgqc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gppxgqfiq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gjiyartdl.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gixdunsam.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gzwkxbxov.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gkrpdoxua.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gvtmebnxi.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gacjsymep.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gjlnhgbzl.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gsjzumqcw.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gpnnsibbl.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gkqmznvzo.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gynvavlws.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gwpmrsunq.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gmfjieehm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gduazoszs.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gegxymudd.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gteywqzkf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gwyexugcx.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gzkaxrfrm.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gzvfpzgyy.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gxqrhfnee.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gmjpraiqg.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gprnfiikm.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gowdydeld.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/grpmggmfz.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gxitlgkjy.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gwjtpfnmd.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ghgkzpwce.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gzgmqttdf.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gnostoojj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gmhrgozuc.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gsxuuhvno.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gfyovveca.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gvxvbtvor.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gzdgjmcix.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ggaomybsj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gwbfbnsyu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gqgldubng.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/godqavbuu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/guhlaqfdp.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/geefjrkwu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/ghzrxtqra.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gwvykqmwl.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gegtmlevp.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gbhyxnaqp.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gzfytgxod.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gksvdzogb.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gfhutawqn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gvzdiobzn.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gufcfpygy.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gkasmtyab.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gbfsvftro.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gdziasvdn.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gojjiqbwg.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gwenfallh.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gbbdhrwhv.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gkmjxlobn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/geipafcno.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gsqmlxwzi.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gfihpzbaa.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/glogspbln.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gjoxopzpv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gigemlbgy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gqojtcszm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/groinxtfl.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gofcejjab.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/glmmwfudj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gbqvspjyc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gofvbwlhn.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/ghggrowtt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gzfbcvnxn.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gcbkgekzc.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/grdqzgzfo.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gdfdkyaiu.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gtmagpghf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gsgvqjiih.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gosbweisr.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gwhugfpdk.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gycgmuwkd.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gistpghgo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjxnjztig.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gidwybtve.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/guvwwgvii.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gwazdxkbj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gfxzfxhrd.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gqpsqdnts.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/ggbgedqhk.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gniptdkha.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gfgzuyoeg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gmxpcmrfl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwnwoppt.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/geudsgdoq.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/goddhwlgf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/giprzojri.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gshllliok.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gqqgibaxd.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/geafgemui.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gmvhydyob.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gbgocempy.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ghcduytpt.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/glcntabop.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gpyiosdlh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gvfkvgcwb.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gywgbbjda.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gqvpnpfio.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gvgqdwxvl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gqfhenzbr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gyiwuzhoy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gjzznhxej.sHtML


<!-- 参考信息 -->