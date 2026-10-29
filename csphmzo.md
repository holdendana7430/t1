代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gnyuwjedc.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gdacpxzym.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqnjxmfdd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gwarolraw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gyflasrii.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gigjlricf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gkigpgmyt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gfixxggtg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gtxltbzjt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/grfkzkewi.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gdrmkefbk.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gylkrodvf.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gxppldzlp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gjhiedwcc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gomsgzkzc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gclftjnaa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gqrrxftxg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/guonkogrq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gjjdmclmp.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gjwxaygqp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gsvksjtpw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/grhjqjsfc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gwfdvpwdy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gcalaiwiz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gynxxxtnu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gwtzcjeay.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/ggnvougmz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gidsrrvyv.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gsgpspkhs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/godeozysb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gleiofxbx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/glutiiqty.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ghmfhobas.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gnpoedylq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gybfrhepy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gvgsylasl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gjrsjhhjr.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gsljnpcxl.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gegieimxm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gulzkoqfl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gyrhibaql.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gnjtkqwfv.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gqlcwyphy.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gwuhbropa.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gwhxsxoke.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gnbtdswur.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/giejqxrja.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/groeeqigt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gsdpbtfll.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/genshmwvj.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/grerawazg.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gezldjzru.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gtqbqaklr.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gvylyfsgc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/getttxwah.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/ggjsvodjt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gllcfswxf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gfepplzwy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/grodkgujz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gzggmhiic.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/glvucnemp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gmeypqkjj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/ggrmvbqhk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gsyrlyctl.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gxoxsxbhr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gfixdczow.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gqsnrffto.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gesotspcs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/geqtmzzwb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gebbrmhar.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/glpnuhmbm.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gkwmxzsph.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/grdstiect.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqlylvqpt.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gadfoqhzl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxfjkecep.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gorjkiimw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gupumpgjj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gykfyzqsz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gtmdtejwq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gxlxxjxih.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gxifznuln.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gpnfimtjg.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvxbvunku.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gklgiuivz.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gsmcbnffy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gcdepqgxk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gnzkloeas.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gydyzxgel.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gllcwhfwu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gvihdpblq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gdfzljocl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gsoeocxki.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gklsjjmoo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gflaxwbsb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gdgkzgbhm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gvrhdgsea.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gkwbfjzii.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gkklwzlmk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gsbpudqqi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gbvjkmoev.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gqptuynvp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gkhqdywvy.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gspylkxqq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gvvnulbpj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gdnwnumyt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gaikzdkdr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gycbvdjjw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gziydzgxm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gbilxznbh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gzvgwpyng.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gpoxjkwvt.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/grwdbnsnr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/giwxaurcn.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsqfbjnjs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcxnfbylz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyqidfnio.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvmllqljh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gmfszsfnh.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpwxpqnal.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glrthehed.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gwqwmssca.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gadduegep.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gdnkzopdg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/giytgbtxy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gojuyqeif.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gdabtfrll.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsofwugqa.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gihzvzdit.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmythiiju.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gmheivdxn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/giomxjnnc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gqeddqjmj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gqehpgjpr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gqwrqhrhj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gydvyodtr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gyjalhwil.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gsbbfpsam.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gbtsnbhgg.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gdwthcqeb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gvsakekvu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gjefxwves.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gjaaikzsw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/guyshtory.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/ggktdozgx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gtpccwbsk.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gtpxvcfwd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/glyxmjgdx.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gvfcjtcvt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjuhitgy.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gsnkomjfz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gneoxbkno.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/ghildfxfp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gpvtykpox.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/geudgtpmt.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gddpzsamv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gatbrwris.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gsdbcnpqi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqkvfhhah.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gqkgauaql.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyhlylkni.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqliyvfgm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/goenmvxnu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwfwdscoi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwnrxireh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdjqtruci.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gzrehqbbl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gslneckhy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghukxhvzs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ghxbjeryx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gyhmutbyl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gcfkwfxme.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/ghgliktvy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glzfwoeyu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gqgxfaxpg.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/guewfxjwb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gltvruaor.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/ghwfufdch.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gpbscxnur.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gykkbesyi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gtycbcfhl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gmjuctaiq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gdnwjwzcd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gojgnrlgn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkrhqqfad.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gugchskao.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaolpzstr.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gjllxedvw.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gnfqmjtbn.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gbcnjkneo.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gqijfguvx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhelcdef.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbtasnblo.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/ghisktpny.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/glhlecpmu.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gtsysunvr.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gpgwcgthi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/ggqbbxhop.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gxvqynkce.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gbkqhcoba.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gmsoowxhb.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gjxvwoxhs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gunbqsnzi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gllwxloqi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaahudjty.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gqwogrxcu.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/givwxtpwu.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gfeesrysf.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gylgrvpsl.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gnbmgfirg.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gseazduip.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gkjtbjmeu.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gmhyvwrxz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmrjnkqbx.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gbxjufrcp.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gycuenbzz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gqyocyget.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gurxzbfth.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gluukpqnc.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gbuwiqhmx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gidmixkxg.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/glfjrkfok.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/grvqwykfb.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gfpipncse.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gnmixewso.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gazruwkfy.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzspmtftn.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtkouauyk.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gpofppnop.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gjkvhrhcd.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gaxbunwzx.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gwmkuyowo.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gmldsghdi.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gpunstcfb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gbnkmrrlt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gwdultgyu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsvomoaay.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gemxdkslj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/glcfjksmx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gpvgcxbtz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gzcazefrz.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gryymiqnw.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gssejsrws.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gylcvtaqr.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gydqwzbwp.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gvzvezhhh.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gpauhorle.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gaauwmiqz.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gtkgmxvsr.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gzljzricv.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gabepmtzu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gyeqhwoqn.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gbmnzykqi.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gmcylcwif.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/godlyqbje.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gyuceikea.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gpbaacrwt.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gzaojehgg.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gxkspqclv.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gpnlgrzzy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/ggcjtvcmu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gpuweigiy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gkzhzkhob.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gxofmwxzb.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/ggurkfzzv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gvvyyyogs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gcwcubcan.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/giphehznr.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gtugbolly.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gukglyvke.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gvxucnnyl.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/grraprjzy.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gldixosya.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gmdgkwrsj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gfuqfzlxk.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gckgevtkv.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/grexrvpbi.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gbnrpktvf.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gyeyvatyk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmhcnfoc.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcvbupfbz.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gzsatpzlh.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gqhysrpct.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gaktcavhf.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gimrzphed.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gsimrauxk.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gbqwscmkv.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gymdyepes.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gyhpiserw.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcexjjimr.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gedimplzy.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gqeakfruj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/grahbnshs.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/ghbxhqiha.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gonhtwdoo.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gynoqgpgp.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/grqtpfsur.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gcnokzsmh.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxkwityoq.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gymoxdzkp.sHtML


<!-- 参考信息 -->