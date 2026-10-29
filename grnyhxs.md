代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gifubqquz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gvxylbsbc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gbwrnlfol.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gmezhotyf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/grgauwhdg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gpscscppl.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gspdizuwn.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gedguakwa.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/ghttubimy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gxymuzbly.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gpustphxy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gqncyhpjw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gcvzjsucm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ggwlzlppw.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gbdzvgenw.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gzoyqnuau.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gbkgkvdfb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gqcwhdisk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gdtltvnjs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gbzwmergs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/grblsqyee.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gvxghqewo.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gpfrgnwzk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gpsrdzpru.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gjjzfeesa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/guqbzubui.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gkhpormyg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gwviwahsh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gejafrsrz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gnlsrjkyu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gwbpmonva.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gqjguwsnc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/grfoabdku.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gyusbetbp.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gconrvdnd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gfmtsqyyi.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gqusjqguz.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gvoxnfzno.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gedcqsgsu.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gtkqlmgoa.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/grozyagit.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/giebigwxd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gnhfsjldo.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/garkufnjp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gjbsdptkp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gsklcaemb.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gsrtormsl.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gumwzwccz.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gyojnmypp.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/glgxloqml.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gozjscccs.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gxureranz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gxczhednv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gieucuiib.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gnscfoqdp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/glaqedebx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/geqlopgvq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/govmkcjdc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gyqxjcgvw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gquwspabc.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/guknwnnsn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/govkwbbdv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gxfeinmrw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/ggzznfhoj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gjvgpxrhs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gnqgwqtjw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gskcbwjnn.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gnqdfedih.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/guqwmojug.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzoctqtvd.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gkrzelzxi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvdehoezi.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/geahckknd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gqnsfnmvn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ggwfkonkw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gcdtgqxby.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gldgpyrub.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gdjbhhwit.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/guvclphpy.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqxotxths.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gimssfgfb.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gsijgfjar.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gxfgsuvky.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gbbmfxghh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gbcaviasy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/goznurhfm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gcawjjjqg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/glwjqfftl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gxebaztqr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gqyshzfon.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/ghzswrgss.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/grkrddkti.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/goiujilbi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/glvpjkepa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gotfmfser.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gfgmcfhjz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gxmqtuekc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gjgozihbj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gcwssmmll.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gzivagipn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gopvrejyd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gezxpnsto.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gczlcjkzp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gvpdegewa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gtsariehy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gkfhhsixw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/ghulsjejm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gzglszjxi.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gcaulokdq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gzlgpgtki.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gauklpiuz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqdnelpgm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtachxyuy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gtyxnkusx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/glffytcxz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gekmnkusr.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/grbbjedhy.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gpdxskgck.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/guynqlmyv.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gqyppqlsb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxlmdooyl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grsxraxcd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gqfvlepfu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gohehdkok.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbbgylzgh.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gcnojxmih.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gulqaccfi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gngxwbyht.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/glgztcsmn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gtfszhtjc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gjtcatcjb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gxtcjaltb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gxmvgjvjx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gyrihmvvy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gedscpdqi.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gwjujgrmj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gorzkhwgi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/guxfbkxpj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gudibimlj.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/ghsrmpuej.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gaytwoknt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gtftqwtlu.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gbjmzjaqu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gajhmfnvh.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gwnxyopbi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glqhwxkbm.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpzqvykef.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gvvpmwhba.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gmfscsbup.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gegjeqnzp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gdizgqmfu.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggxmgnxwl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gkefpnasp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gpmuywpgw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyotfjrcw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gfxwavjll.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gbyrdzklv.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjemukurt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gejujbool.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gttcmtuph.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbikdxtke.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvcheadwn.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gvpcluejr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwqgmvgse.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gltvftpjn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gmljhqliv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gufwmmtfi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gatnwrrgy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gmlivqtuk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/ghcladpyh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gfygcfkis.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gbsbbdlgb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/grgxdrrno.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gpswjuedf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gnxnkunqd.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/glimhlclj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gcuzcvrul.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gocgemmal.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gvobjjpix.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gorbjirfx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnhweoisy.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gdjdisxsx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwkupzaud.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gyljkahdj.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gpwsxjlid.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gjtqapyqc.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gmzmuzcok.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gzjfnwffr.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gjxeiazka.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gujoeatxz.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gankehiax.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gaixwthgs.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gbdzdoyjz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gdyfbzudg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/goberjgyt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gepxxrnrq.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gunpqkamj.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/ggrshzibf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gorhmaadn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gqxotdefq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gphxezlyq.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gysevviup.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gpdrlloao.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gibvjjckk.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gudvtxfvm.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/getyrepks.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gajgmjvng.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gmbscqksc.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gkapdflcm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/glwhhcnnt.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gebyoonww.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gbsbtwxpp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/grvvjifjs.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gftszsxax.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gyyrxepnk.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gymzrtlcb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gxvkgpijp.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gbxyqvlxh.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gqhokanmt.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/guefhfftw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gsbgcrekr.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ggotsjqpm.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gpdvslmey.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gegqihvrn.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gamxoyfri.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/ghpxgojol.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/grgusbdqc.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gadgdvaqu.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gqmpddfdt.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/guhbhxvis.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/glhswpmeq.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/genjshuig.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gchtsuskm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwicmgdqh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gmxtznmpi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gnfjmxoio.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gxunqghih.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/ghqjmxmfq.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gerzssovx.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gsyruwbxy.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gpzkaojrk.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gdachlbqd.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/glymezgjq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gsbkimoll.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gjnbjzasd.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gvhlnvjlq.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gursresni.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/ggeysoshs.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/goufmcobv.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gqngpzbpr.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gpaqgbddz.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gcvtqcmmc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gzjxawogi.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gjlolemoz.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkltaxmef.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/ggzhcwkyp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/glwcfjutx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/grbadqxtc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gqkkumigs.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gmixabqaf.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gptvlyplj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/glcamdntw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gbbxhpuok.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gkilusgwe.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/goslobzuw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/ghgkuetkn.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gkusoekdf.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/ghgvqivez.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gvupdhubh.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gigvbglzd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gadsmbpdz.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gbnomzsbt.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gvjwgqhkr.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gqygsoyys.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gtgkpnptv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gxuvdwytx.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghigtimqt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gsaaevenp.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gurdjgvfb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gkxoepuml.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gvmionmyw.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gocfhzbbf.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/ggwzdbqcf.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gosddaxzw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gndpujkuz.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjbmbkgsr.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gjejrjwpn.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/ggauzgyue.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gnxmvqgnk.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gmdqhdkhg.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gyxjxrnwr.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gjlgztbja.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gfdtycxuj.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gtqifhnlz.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gknpixutq.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gbyxejaja.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gdvqiugmj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gslpmmjhd.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gmcowycax.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gpjqqxmxj.sHtML


<!-- 参考信息 -->