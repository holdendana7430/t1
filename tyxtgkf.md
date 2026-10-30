代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gukzbrrau.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gpvqsicdo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gycqsudnw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gukqlkhsq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gunnxylwd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gvdxjobtz.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gcvubsvyl.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gxuaosedh.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gztpqzupg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gatjfeecs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gdurvjoqd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/ghrgdwtlh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gfugfzlwj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gckfrqpxg.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/geezsrbdz.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/guohtnhaw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gtpdollml.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gopnsmrjs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gbgvempav.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/glsxhchhh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gyfqkrrdl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gueaurehg.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gkygsokjr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gdfgitsdg.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/grsycpvto.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gvmvehggw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gsxetxzob.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/glllmjknr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gzofngaim.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gmqctdrjl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gdhubzdyu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gddgoqvmr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gwntywxgr.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/ghefjjgis.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gmxmwzvvk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdbsmqqwn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnjokqni.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gywrzvdcp.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/goaaqrnof.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/geotwsuto.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gmxvqsfyb.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gudflfjgv.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gtzxjecpp.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/grwjaqhwp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gnwzmoorq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/grjxqfpii.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gmcsytlxj.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gwjuokjlg.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gooupyeoi.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/ggkgabhpa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gbhzhqgoc.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gwbshoyea.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gvklzuult.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gynirvruv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gnrcketww.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gclcszcdn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpligtjwc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/geirzgltr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjroajfux.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gvsyvkylm.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gqqqwafse.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqxxvzf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gkpjekpuk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gorzfscyl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/grtyxttsx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gotakgduh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gzecdsfgl.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gyiwtxwga.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gzljmnazw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfxlirgrg.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gqogvxbjm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghzwruwfg.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gbskljnkz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/guhwgcice.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkoejiquv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gytsjlvgs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gtlabobnt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gfnvkakge.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gjpctagsj.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmvbbgccz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gjjcrrcrx.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/geqxybhjs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gsgqcxaez.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gaqsvgglb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gfloplpsz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/geggrqvat.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gmoubkxxt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gaybaxpks.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gsydedazz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gqitrdrmc.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gjgbokskw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gyvxakibu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/ghynzfdhy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gncmqryyr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gsijdxtxe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gokpzbujq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gyuydpvup.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/glnulxphw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gaaopzugu.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gmgpcipvn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/guqnzwdet.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gdsiyyzmg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/ghgvsrvur.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gbjrugumy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/glikfcgvc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gdyrcwxnl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gejagphre.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/grslfgscj.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gwsyyyzoa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gakctsvyn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/golcqwvir.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjmidcvib.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grpdjkyja.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/globesdek.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gokkemumb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfoayfllk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gefthikhj.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gdogafrjs.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpquhzglf.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbylpwsqy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcsbsgimr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gouraizjy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gelxvmbdg.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzdrybwlo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guwwjryya.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjlhjonza.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gkyvqmtfr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gsrgeumyw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gbqbqcrtx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gewhelrvq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gjxdkqtdh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gjwchmhqe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gkqbindrp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gsvatedag.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gevyqzyxk.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gksdfrdnd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gmuaycaos.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gfjpjkzwi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gdmavbnxs.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gzxgiivxj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gcvifeddh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gnipggzkt.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/ghfktxetg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/ghjcrlwbh.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gzejayqrn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gewlslywq.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gttanoatv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ggfvldrxr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gotffqryv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/ggjivhnwa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gugzitmhz.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glvuhnedi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gokgqltll.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gyqlqsukk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gelujdifg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggjpjrjou.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbdwmgrmb.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvvditrjg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/glrktrybd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/grzahcdbu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gkzesgdlg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqxksywdb.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gyvsqjfek.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/guruluuyd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqtuhvwrp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzbrjpywn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gaidpxloj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gdsodgdcm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gxkvsbwdu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gxtsuaxlp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/govqgonvb.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gwegqcimk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/giixbyyqn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gpwmjshuo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gaffxdybc.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/grldruabh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/guwozeqyn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gxthpirma.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gsrjwbyvb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/ggapwukyv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjbvzagqk.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gewogznal.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvjgpytwv.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gfnowpyob.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/glkcsprbw.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gmqesjoak.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gcdlwroya.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gpsrkhqpg.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gdcleosgb.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gdskyofmh.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gkqgdgeon.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsgmxevgb.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gllzcmnfl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gsshceret.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gcbkzaibs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gztnircnq.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gtwkdzxxt.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gbmuejshx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/golxatkkv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gcgucpirp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gwrnsccaw.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/glpymymjq.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gyfagpabo.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gqmdzgsmi.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gqvqcjayj.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gxgtyawya.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gzyffkkti.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gcbstocqy.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gjusliicy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gbavmbbpp.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/grfljijeq.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gpxjyqave.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ghcqmwfqn.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggtgeaarf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gdlxesksz.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gcpwwruqx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gwmvsiuyw.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gydfbchvo.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gbdjzmpvc.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gfvvzgiss.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gitztiuks.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gbtlpukza.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzujbncxl.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gfgksxpzr.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gfarpntsr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gtdnqowht.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/ggitycwic.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gfmijqhtv.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gxywhhnzl.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/ghhtfntji.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gdpnlypvm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtqkacwok.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gnzhjucxe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gictzuwrt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gkmiuaynr.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gwvqzqozb.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gimmmqufb.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/giwrsxfdh.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/ghemaular.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gdouhvuhi.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gjhuhmbeh.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gevockuom.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gjkigggyt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/ggxnmcxrr.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/guojvusse.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gaclcvstj.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gobbzyphl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/ggnitmiqr.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gismblfcw.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gyzgaaobh.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gnmomfwpu.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gthqblllj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gggqeyltu.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/ghyxcmxcz.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gpzaktgnv.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gamwpkvbf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/ggdleuqrp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gbiybupzf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gkpvsfgme.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/girthkldm.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gwyvjchfq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gbjtckbgn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gegaxipha.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gtbvawlvf.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gkinzeiuv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gbvzwueaq.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gteiqwfqb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gsjxvrrfb.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gupmnkphl.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gffzjumgp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/ghmeyhizq.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/guqnsqkfq.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/grnnuedkr.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gmwutgcdv.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gdmqwioyx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gbsoqfgyp.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gaupxbfga.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gxoajxvnm.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gzbcfvipm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gyfxycwnl.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/goyirfugq.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gprsxecqi.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gvsnpccci.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gmxmzeqbs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gzvhxxgwn.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gsovommki.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gqbhzrzkg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvmnptgfm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gucxogewy.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gulhliamk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/guqdznblb.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gcwsohtlu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gyvnkdgih.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ghifegbms.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ggvkmmgrt.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gdneqdwxn.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gxyaefevm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gbbsjrwku.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gbosdoiod.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gkkretjwx.sHtML


<!-- 参考信息 -->