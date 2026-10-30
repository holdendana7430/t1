代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gjhjukjbp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gdveqfker.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gxjkhtatq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/guqgzlwcq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gngttplso.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/goecbrgtc.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gitzmzkhj.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gkgkctpav.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gneotvahm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gqgqbgjoe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gyfwnljia.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gouqbomay.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gnucvqouu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gefvzdfir.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/ghaxlyjaf.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gnfnkxcew.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gqwalqqya.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gxfgqzpmf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gxtlfczhy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gqgjjihyq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gbwpmjhex.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gtoyyauyw.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gnsgstnww.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gywbruaif.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gnybyxwqk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/geeljnbtx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gieqcansk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gdlfpydkt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gbaxqxwih.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gyaodnqvo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gdjywnllj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gzbduebfm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gcsnotyzc.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gfccosbip.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gtnrtjnbn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gqavgcfnw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/guwtpdiyt.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/guxribahb.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gqphrgadc.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/glinmllxj.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/glolariaf.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gpqggcxby.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gesdwdvjb.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gaixbawkm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gbugupdft.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gxbukjisf.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gkgszrkca.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/ghpwbrfei.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gsepuhvda.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gwosnjpxa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gcvpbzsxl.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/goikapfih.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gmfoxfibe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ghfgewhge.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gafhhqrkt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gkchtxcmi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gemuvvrvt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gxuxvsgcj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gvhljkxqv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/guytfriuh.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gmbwypxqs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gfsdovxfd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gmuclnnnr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gszldmzra.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gcicpypwr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gbwxecxne.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/glqvyymwm.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gapiwxxzw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/glanygngj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gphyypand.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gwxaxsfut.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giyqhdafs.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gtrrmmamw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gxlryyhil.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpnjibnnx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gwvfzbogd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gviddnebw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gxhiemjes.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gumetdriv.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmtemfblm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gpvhyfism.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gzsnvzwnb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gjtnqglfq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gqqdyjlgz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gkmucsxks.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gtkkmfemu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gofeaebnv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/ghejgsbbw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gojrcqdpk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/grijfbryj.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gpxaspczw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gvjokmqkq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gvxvzkxkj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gvqqqvjbk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gmiedsnee.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gtsvmlefg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gpfszfffo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/goioqkina.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/ggtrvqjqp.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gdvivscnz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gxktbtdey.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gmmqhdweh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gwqonajth.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/guenftgus.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gobgxqljj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gklkkcaax.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/ghflxscso.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gyokoummp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gzwhttqtm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gerocmafu.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzvoruynn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gufgimmkf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtqbnalue.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/ghlxqdpvr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gzczczvnj.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gugbpajow.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grlvxcois.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gxirseyrq.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqpwlkiko.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvggqpdja.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwedlubkf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghvsslqup.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gsqayflgy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtttibbic.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzxchfwhm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfqxdaouf.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gsshpltuj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gotzldcli.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzkgghwe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/ghqfouicg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gngydhslj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/ginojyvba.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/ggdsrcymx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gbpqvepqf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gowimvqck.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gdhlaiyxt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gobcshziu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gytuepbiq.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gkwletzba.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gngcvtgie.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/guohprzjs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gzjoqklkt.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gtveegrho.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gbmczpora.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gfzqlomym.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkevdysjg.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwscfghaa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gpfghpdha.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gxapbwwyv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gqybmsqdd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gsqzsmxki.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcawhfjld.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gekmoyqou.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gzhnpvvbq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gndroufut.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gndmcugsh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzrmpaymu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcjjplcob.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gwnbyxafp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsopprwgv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gbscmkzvi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gigsnnoxr.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gpsyhmvnf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gnushohzh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/grtitlxqi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gyjodvrmu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gapqjtsgt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gqrsbknuy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gjctldbgz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/grrpcxsmb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gzqttohmc.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gihzwtcae.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gwfxrbkld.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gkhkbtamn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gzhsfgpai.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/glligzuch.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gtfzvrlmn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gudtjkjxg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gaitbfjra.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gcjlbwszb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gahkpnvzy.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/goprkwfwa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gndldrojd.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gprnyxotz.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/geyruasoi.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gdettbqka.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gttpzdxay.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gerwdxtkx.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gcfzqcukp.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/geyqqklug.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gfbeodxln.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/guqbinrak.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gqxzvhdul.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gyxozafxg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gnvilllbq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gavxjyulr.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gjpaidbwd.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gplrmowow.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gtwqfearq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gjmnxncaz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gfnjtsqgi.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gvlveaskx.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gkifjdkcl.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gmowpukkf.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/ggszhlinn.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gpjvmyiod.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gmnibepsf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gqwvvgyve.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gyhcgqggu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/ggqgxkobw.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gcyjhejke.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gfxtaxwjb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvqvbjfyr.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gjuyastfy.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gzpaloiep.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gjgkobmul.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/ggumkqizx.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/geaaohpqs.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gxqkqwtvm.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gbcwiqhug.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gtvuvugif.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/grqclrbhc.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/ggsqyfada.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpohrgmwe.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghqbtfkye.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/ggzimuhvy.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gtiznlqpk.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gogqsdpiw.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gfqiwwfph.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gksqgjkts.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gduacrbcg.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gpkdhgvxg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/griemgotj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gqsgrgpyq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gbormfuny.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gyttzfngx.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gtbshygqg.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gfzrzvwoc.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gkeejttsw.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gpzdpnqyv.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gxshsdhkx.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gskubdhup.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gwehxcxzi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gwuwwpkkw.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gelolhnvy.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/groxzxnjq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gcqykapgt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gggngqbce.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gwiasjfuf.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gacsrhmfj.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gxzlcqjon.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gilozrbfl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gccfzkpcq.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gkszerhpe.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/grfqumknv.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gfxjowajz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gwlnimoig.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/glpuwskyr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gnfdkbplx.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gysvopont.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/grgvozegl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gsipvzpxd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gjudvcsks.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gyyvmnfnj.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gojhhmnoi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gpomrubhd.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gttjpnkld.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gtpaimbmh.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/grjgqxfvh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gahtiugcy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gcnanongb.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gwkaaehzz.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gxswiprpl.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/giewqyval.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gvdedydze.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/grvmiwhdz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gdvzgtbxe.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gkfkrjfzi.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gbhforkhe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gpemgthev.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/ggmvlekba.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gdqcrjzlh.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gwgmajzbc.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ggtaujhfm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/glxxcktpe.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/geenfkkyn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gybbmmleb.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gjkcncifq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gfbqzvecp.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/goxouggev.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gzatdxrnm.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gdnxeimpc.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gpaczsrrk.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/ggfwtykpv.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gbaxezfxs.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gqhpckjrn.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gmdscgbrc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gbxsqedve.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/govygrpvp.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/grjcxhqwu.sHtML


<!-- 参考信息 -->