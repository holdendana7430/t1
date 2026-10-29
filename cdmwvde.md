代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gzjhevgfc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwujodccd.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gvbfekzqo.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gppjpjwdy.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gnnjyxazm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gsttwmwdw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/ghgekarqe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gcpzkdlmc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gdcubhpbe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gaokmtipm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gzsmrfhqj.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gwpkrlllu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gexzwifjx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gccqlhyww.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gktxpqcez.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/girzcygxc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gqhkigkyp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/grpsnmxuk.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gfifsknkw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/guivmqptb.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gixhgxplv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gnxbjfytq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gpnehpkze.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gleaoeiac.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gnanzpuqc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gjekvjfrq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gqoceeguj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gcxhrnduv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/ggcrgeydp.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gikdttvkz.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/garpjakrl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gifpjlnrs.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gdpvfclzf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gycvanpgy.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gkvqwazoy.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gpsugwers.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gzgkrxjyb.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/giqxmulef.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gddmgkwyr.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gwwmobepe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gbcqwzngn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gytexgnhh.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gvesqhasm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gxqjamjsj.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/ghmdirtrx.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/glcortmyg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gczqmdtzm.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gferdwlkx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gajyfwxwy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gtevgmjhz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwyphvtkt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gdbuxypbm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzvluguex.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gyqkjrvlm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gnaootlez.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/guiwkbebr.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gdhxdtecc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gtboevgwf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gvekwzwnf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gyagylwit.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/glrezfhpq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gbaltqycq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gupgznmva.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gbnvvdwbo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gvqbyrybs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gntkgxoiq.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gxzrmrkgu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpvrmipbf.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/ggyqzuuri.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/grpybjffd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdxbllfab.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/ghrwzwwfd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gvadqidbl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gqdpctadl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gxmvtwdgl.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtzhjwgof.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gzznqzqje.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/geanoawps.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/giptezrsd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/ggzitnhrg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/giuykfkkg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/giwszxucv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gauattmhz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gadihnmjl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gjlsrxnsp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/ggcascnkz.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gkzpurwac.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gdqoctjol.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gzfoibskd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gfbcvabra.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/grojzdrnj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gtqgfjjdn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gndbpzydr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gvrbpmafb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/grqmgvgpa.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gzwwsfgjg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gmxdvcnda.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gkvxzmuar.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gvmopetdu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gstozcppa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gbtolilbt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/grxtiwzap.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gtdxxslmg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gwkksulks.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gyminkmnz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gaqsorpwz.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzyawebik.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdcrcqaor.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvnxbaewp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gsupinbdw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gbzllcicj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gngcdaexc.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gipdhgnnq.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gaxlyqwfh.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjdapmkxj.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/grvylcqjb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzrrthmvd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzldlzqxl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gwliivyvk.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gctjkwpae.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggdnhdhyx.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbyrhxbfh.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gcfcyuxct.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gxeaomgqn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gjexhyddm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gzbkqnwvv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gayuyabfw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/ggtaftrll.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gzrzkxobv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/grtnjsttd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/guxcsnbxw.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gnvtslnyk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gljjxgtbp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gellwxtyt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gszszmhfp.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gzswagria.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gbabhmpim.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gupnoqcbs.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/glojzwgyj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gwmzcsucy.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/giysxuzqc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggrpludap.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gctmywmdk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gbkyayiff.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ggrsyvcfm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gfgfykyrt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/guazfnxen.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gacsmptkg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gtivgjcdo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gtmlpukhk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfdcvsiuj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gqjlgcskl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gowwphebx.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/grgbdwipn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gprjszblb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/goxcmzebw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gncqkuoqa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdsbcaiie.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/guvpguzhx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghaardgrt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gvxtjjaan.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/grmtfbtka.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdkgsqjfy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/grvzmlwis.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gpblufcns.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gprzbrfnm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gfajbhrwu.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gniabyghd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gqlbhoqim.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gbwghilqv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/ghermdbnu.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gdfszxbnm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gnbnieyij.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/guytqybcj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gzzclyxsr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gflohgznp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdbepzgsi.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/grygidpze.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfhsudpaj.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gmkuhzqzy.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gwcrmppjh.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gzvgzcydw.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/glirkdkuw.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/grlmapuhl.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gekbtjbkk.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/ghgxrwdmd.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gxaiqqvkh.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gbwpksdzh.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gjszpeuxk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gekkgqjgt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gponmyapm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gzbdkyfxj.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gjxufnqdp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/grbrppaao.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gtibnsxrz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gdynicdhw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/ghjgcokhw.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gjtnystdx.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/grypctpwv.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gjwkdxglo.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gwnkrtinb.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gcwrjppni.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gfmffmpsi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gfwwvictp.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gwrspazjg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/ghtyfanog.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gcozsdjvf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/ggtsjfbcw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/geyzwvhcy.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gyyglrbcv.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gstiqwdms.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gkrccshoe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gvxhhttze.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/giwkqtzvd.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/geraeppmw.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gpntcveas.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gzjpwhwbn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbppvzeqf.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gjmgctklv.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/grsfucghl.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gakqjhrss.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gorainchy.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/goevhixvw.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gvifjcxqm.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/ggenweagz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gvkdedkpb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gjmbnfgyx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwcdhdvwz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gibunwlse.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gnhcewvsa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gepujllff.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gzviuqctw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gkfltkzwj.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gqakftafw.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gbmegauku.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gppsyffdl.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gexceplgm.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpxlleuvu.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gxiobwmal.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/galkfvfbn.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gyrgjyvtc.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gqtbmmxls.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gdvyyscaw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gfmupegjb.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gxwqmadjr.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gvenjsngw.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gmkgwqwor.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/goqgbozpr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gygnrlqwx.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/ghldxwhsl.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gffsvrdzp.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gyhrmkpdo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gikhoujbv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gvrabycpv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gpjgydsfo.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gdwxzaupo.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gfdmoogtg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gncbxxwwu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gpnkgujzp.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gdgdvddrj.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gndogfzoq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gekhthubo.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/guaycwpht.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gbyxrxhvv.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gemoippnn.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gtkrdrjwq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gczlqtjgs.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gddndrmfg.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/ghtbkiuxg.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/ggtdbiltr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gactyujua.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gpcsgwdhy.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/ggacaqxbr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gcyyzotkr.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gbzutsaey.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gcxsufkeb.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/ghldonbjb.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gjectzqhw.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmuvqqqpb.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/ghyofugau.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gehltesas.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gbncwgpfq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/guxhmwjqw.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gmwqrjnjd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ggyoqkvcz.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gbhqpcdbp.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gspurxlai.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gfiwnauou.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/ghpvieiwq.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gemjsapxb.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gkbuxzwek.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gdyiugtrp.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/guqpjobls.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gyhfxsrgk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gmneuygah.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gwddulxmr.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gwezhnjid.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gxbuxawqz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/godmdgqyd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gcjdukuhf.sHtML


<!-- 参考信息 -->