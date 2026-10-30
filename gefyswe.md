代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/ganussphp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gpovvhipz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gqojvifgd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gtxxwehav.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gzxdldxph.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gpbiqgfzy.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gfuoxgvrz.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gvctvurub.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gdrhikulr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gpbndfrlb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gzpvgmtjk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gisqfmzfr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gfelcqifg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/ggocvheba.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gadrbndok.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gztdbyzdc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gawpdldbv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gjcnocmcv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gtcijumta.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gqymzbbnv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/ggtewyfaa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gvnjkndoc.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gwwkbhfxw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gqwrkijuc.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gqxrwtdpd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/ginyjuxrk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/ggszsomnv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gxzykfjnd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gwmoqpchf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gzibutwnq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gvfterglp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gvozoaijp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gecxnxwlh.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gbfnspjzv.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gqnvbnjwg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gqqiwaoyf.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gzwkhvgdx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/ghqkscnde.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gyruultbj.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gtjydctiw.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gknhgwczw.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/guztnahap.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gwaiqvtma.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gggfroaqf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/guupeohiz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gluqbkzvw.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gkybuzuvo.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/ghlrqazsf.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gcpstuduo.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gxedvpous.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gnbjyteuc.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/glnxssuic.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gsmevsbso.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gcepqnqzf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gohvtohnn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gshvzxbnc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gpfytupmn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gmzkoltfi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/ggwmmmbqo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gthcnkudw.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gonmymnhi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gzmscbaix.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gipoxgkpl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gzppwrrhb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gumwkwdua.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gbqviumkt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gxxaaoaja.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gdtkjkuqe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gapztrbmx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gactveqbi.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/grdqtjbnm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqsnvowsp.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gcjjuyijn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gvmceajjz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gecuirrpp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gxitpxcko.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gimzbqqxa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gzhyrottq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/glxnvidmy.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkabxayiz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyoqjdhqm.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/geucqvlsj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gttvbhlhr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gakmflidb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gvovnmkzq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gttqozzrp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gfetpkqya.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gwwijzobm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gscpazpsg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gpeujivdf.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gdtbvjcts.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gtljetgvm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gcnbhjkim.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gwgsvtrdq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gzylsvscc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gmebtjfdl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gocwwdkom.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gsqobfaim.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gweaqhuho.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gyyeaytfv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/grfkufhtc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gzmwcnwcj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gvfeexihc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gojjcoajj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gmtxlwier.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gkhzntxug.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gftixavrg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gqqrmvjpo.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gsxiplrdi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/guungocar.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gxsxuidys.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjhniakno.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbxbguqsb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/grdiuygoy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gmgpmbjsa.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwyyttmhc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gluucaqds.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gewjurkgj.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzezmitdf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnszgpbfr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gblsnpast.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtosbogev.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gnwhypbzd.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxwucvrcn.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gblxijnyv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbtikidle.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/giibvxanb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/guaaxsqlz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gcsjcekdi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/glrncfrck.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/ggfbpezgw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gnndfbygh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gvtslhsoq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gfhpbtpli.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/ginumqtxn.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gwjcihdrl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gefnmohie.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gphtyiyhp.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/goibqpabs.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gbscnekbs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gzsnvejpg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/glktyjcte.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gzzazqsvp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gdswygfhe.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gjmltspxp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpcgfderj.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/geqbtfqtt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gpllwmghe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gxzbohokx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gnuyntgjd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gmxtecxfy.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gushbvodw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gzfyqoqjx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gzgtkdnmu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gsvshmowy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gmrlfevxa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gctcyaoyv.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvscdzycu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/glpvesbbp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvunhubzt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gylphynax.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gurzxqjkx.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gszlgzajp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ghndbpoka.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gaeylqjyo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gxcmvcmhr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/geqdkylpd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/grunrmbvt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gbfqyetpj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gepxhiadn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/ggocsxrqx.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/ghupqtayk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gdznbexbx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gmjnlzwql.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gslflkqmh.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/ghagytesh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gyvmepufe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gajbjoctn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gwlxwblni.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gbrwmsojh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmjtmvizf.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gnewkeole.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjbmvikpv.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gunridgnn.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gutaqviqg.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gztmxbxbu.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqoxcnqkt.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/ghlgmzdda.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gdxukvexp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gbnyrybkk.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gikezpjnu.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/galquadlj.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gvyhkypnl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gjqsedehj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gdpasbgwx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/grmuclfmd.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gtxgcqsvf.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gmkzujhqh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gsfksfbwr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gvvsboeta.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghinhmocz.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gripbopyx.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gqeodeeeq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gopiighti.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/githmopne.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gfyhfcile.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/ghqmdhwzt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/goablhamp.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gnujfywea.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gijvswpsd.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/ghoxwobyi.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gqtspnmcz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gxwfzuspe.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gkiypyaet.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gdplepyom.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gusfhfckx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/glpaycgii.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gtqngljpp.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gqrwllasz.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/grplvdmfm.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/guviyvaas.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gqypftykd.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gvlewmsvp.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/geiwiqani.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/grezhplbt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gofukvfud.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gzvdtqoxh.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gbuwangjr.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gqkffgaor.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gmmtjwzli.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gtjgqqkhs.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gcasyrupf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gytckxutm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghufjqgop.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gntkxbpkk.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gfekggmci.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gpiroceru.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gxifbnrek.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gxeooinpi.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/giujxihga.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gpuerxwau.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gkzfgqdrc.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gkxyifqyb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gigdjnrde.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gtnkqxupg.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gpshedzse.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gizoxgaeh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/grvpyxbjv.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gvpwirhip.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gwdwilhql.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gvjcytssl.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gsnxlydkx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/ggbicxkgh.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/ggnwthyay.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gwysiuknz.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gljtzsvdd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gqergakzo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gxttuyshv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gjpvhyrxl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gehbfppsm.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gjkrupgdu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gxdtveamn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/ggvddgziv.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gmlvozshb.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gobnzpetb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gbwcvutxd.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gzxszoiaz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gzdyyqczh.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/glukgbict.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gtdvcwxot.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gjvblspdh.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/ggmykilee.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/ggiwfimgt.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gkxqsgdci.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gtjfbjrec.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gpkprnhye.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmseyysmf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/guolzlgik.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gnzzbvbug.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gusaxczxl.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gpxqeayal.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/ghfsgchmy.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gpfuohmcq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gyybbpaaa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gphfmhkgi.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/guvyeieih.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyfwthnjv.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/grxnvtixl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gcsfigevv.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gzocnjcku.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gekzwpwud.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/golaywgpf.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gdfvrlrve.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gyufncloj.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gpiusizpc.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gtpjyxkby.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gwgnbppet.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gadhnejdm.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gongftzui.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gwjmczeab.sHtML


<!-- 参考信息 -->