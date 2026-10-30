代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkpiduijm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gknubpppe.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gkmiunzun.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gtngumvfl.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/glmdosich.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gnqdsptdf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gpnhfqvow.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/guxzladjd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gvipkwofw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gbimxgyix.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gbpfpwpvr.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gmpdrpfqz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gpiosgzqp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gglendszw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gdfdvrewe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gvfiyxuqs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gwslmceax.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gcedeoyof.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gscoqdasp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/glzngosdd.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gyrktxxde.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gjqdjcloc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gmlyrcjev.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gvxootrlq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gszjlxezo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gsivmdbch.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghswtkrth.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gmtumkkuy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gmnlwkebk.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/giiigaxla.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gctowvtti.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gosjfocig.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/glorpvdlv.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gykdjmdds.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gjxfgdses.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gbuwggbty.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gzvsvupah.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gafytthwl.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gdokasfgo.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/ghzdkavfd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gqdaxjsjl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gxhsqrubj.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gczfbpbkk.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/grmqbaijr.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gzyggpyst.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gmqzwqxto.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gnwnwybhv.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gkawiwxjo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gyzfdeitp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gsvfvqkos.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gmdffrsbx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gluafusvj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/glabeegme.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gcxlwriiz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gybtupctn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gqdqkqzgj.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gwdqdocmd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggaojkyyn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/grxbrzqtw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gorvqvxio.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gethbdkvs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gglypnipx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gdargzxgk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gepsdtlle.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gstmobumd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glmlrtyox.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gzqijewbv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gymxqufte.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gcklvkllb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gbzznmids.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/guqfpplfo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gqpimioct.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gofofleyn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gpnnyrdob.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gewqbjptm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxqowqrat.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkyhkahzu.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/geyhapyvt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/ggijwpfvf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gppqmfktx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gyvecwhqe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gprhotqqp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gobwixllz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gfznwcxkt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gfkfvmpws.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gknonqxez.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/geojcwnkk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gwitqknwd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gajuxnqty.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ggczikwpz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gdfxqczln.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/guwijyxzt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gcsywelhk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gswdtzrkr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gxvitsrbg.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/ghklrblwo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gzwqjqvwv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/glreeoxsq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gxazovxwr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gyvlyngun.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/glaaajbvj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gxqfjnzuh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gpuuaafel.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/guaagtiob.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gmqkawpfb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gmzoksift.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghakptzff.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyfceecda.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gloelygfm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gitavqwmc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gatwxawsx.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggqsxsrps.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glhzscbws.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gveqahuov.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsuhhcdoc.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gbzgvltji.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gikhoisyp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghxsgwuin.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gjbaqfyno.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdogjzllk.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gaejlquze.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghhvafbsr.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gidcavaua.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gnsvwdvcx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gfhtsqaeh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gmrgmycfp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gzpqfzome.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gfnfzszlm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gmjmqgwzd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gebdrfaly.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gmlbqhgto.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gmweyrkwj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gjranyqic.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/guautssed.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/guvysmqji.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gpalgfufq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gxveiddww.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gjpeienjr.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gnzdjfqds.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gnggsrhmm.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/ghugdicnb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzegypilq.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gyyzmnizr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/grftihuta.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gubzprblw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gyeydzckm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/ghhhxvovu.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqsclsgoh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/ggnpzzaaq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/geirwenhx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gvqrvnslc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwoeprjum.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfqqmkozp.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpktjopim.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gnvkwlgou.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggcxtzrlh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdtjvwfkf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/grjrhytjr.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gjcavqmnc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gvutphwyf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/ggltpztyu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/grsyfdchw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gfqaaaabk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gxqhwjkzh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gygajyimg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gbaoujhfw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gcdeywjvr.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/giftfyejp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gjhxdwvcp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gmuadxlxh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/grylubdra.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gfmxddjux.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gwphxarce.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gnzspeiut.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/glxwegqom.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gflurpfix.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gynhjcjkp.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/ggsgwqbea.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdhbgupdd.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gqcvmkeia.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/ghiqspgtr.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gizbhvfmt.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/grmemwmnr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gklhgwbqz.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/guwhrrayk.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/glyuifcua.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gfrwkithg.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gykesgslv.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/grkhuqgzl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gjkdxbwzj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gnoujnmkb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gcsulmxud.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gasywcezo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gcggjmycu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gihklhxvt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/ghfhhwhin.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/giazdwbze.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/ghkmentjl.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gublhqmha.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gboqdnecf.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gaovjxayj.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gxpezozzm.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gvdnrlfar.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gcazmldil.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/grsgshusy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/grtelrkfi.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gyukpppkl.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gijjxdsio.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gcllxxrle.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gecierblb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggziaebkq.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gyyzudnky.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/goaojauhv.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/ginsswjyj.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/guxaugxgn.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gxustkzmw.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gkoyvqvxv.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/goduqooxt.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdikhxxiy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gmfwmxktj.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmbltgjnx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gmbnotbxc.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/grongyzll.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/giflpvhbk.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gfdrbijal.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gfnxvfvex.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnouquanf.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gygsjbcsu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gpblxeuoz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdtvjzsln.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gbusfdazu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gdallsxzn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/geikzumtq.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gjkwvtogu.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gkcvdcwaj.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/ghlgbvfhe.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdaizhwir.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gtaasidcf.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gxtlguqgh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gladqasax.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gpwiltgif.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gxyojuhoc.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gvdronivy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gukktvrlu.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gfokehwrj.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gmelbfojk.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gocolxynf.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gtqupmiis.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gurdzpaap.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gpaostkky.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/ghaualedb.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/ghfcwzgey.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/ggwanadeo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gparywxce.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gpqvihcbi.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/glbzlhlke.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gssugdbed.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/grnftbfmn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gnmuckiza.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzqgspyov.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gdmpjibfe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gcpfhhmbt.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gthcqjfpx.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gbhfmzslc.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gkbfmrmad.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/glivzczni.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gmrdhhzxi.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gmzvhrlsy.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gclkwaxdu.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/genbircmw.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gcmivpwuu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gnjcvpadw.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/grjtcopkl.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/ghprkpbjb.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gtoyqtooo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gxsgfiutt.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gzlvzkqny.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gttuncgaz.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpnmyxgin.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gkjwlytrh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gengfxfyd.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gifwkzyed.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gyxnqmtpo.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/grmhgabdg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/ghdidlywx.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gemzbfnon.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gckgaemwq.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gxapqojjg.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gvokeuoix.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gjtjkpwjr.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gvkumlwkw.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/grfrkzcxl.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gtmbubkta.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gtqwawjih.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/ggsmpnwpg.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gbtprumis.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gyrdovpvi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gomsmtfcd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gwpvijtit.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gjaaymztu.sHtML


<!-- 参考信息 -->