代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/glkjgkhjn.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gczzixbji.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxfjkadxk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gewmsisaz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/goxlgxzol.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gwnjzthif.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/geuosdutq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdrqyebqr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/giwoimhzg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gicpiercf.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/ghwbamgsl.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gofmtqfme.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gpsxbdbgt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gxbwhuutq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gvwjzsgjl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gxqzfqsll.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gktpaybfs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/grpkoztoc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gbhpkoffl.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gpvzdanfx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gvyihacnh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gaetcboir.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/ghajnodsz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gmoqfvhde.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gursdhghk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gnlmrhzhm.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gkrgvffld.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/grusxrcfy.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gltuieibn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gmfyplgnv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/grzaafwvv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/glnpjaerd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gikkrsaow.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gdjgvsfbw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqokhblwe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gniprwgnw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gwmicdwjf.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gsiidsste.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gtpgeyucs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gsqvzfupm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcrxjbmx.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gmsycpdgd.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/ghdkssvum.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gmykpgfqg.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/ggylhzcqp.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gsfhurmql.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/ggwpthxar.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gldrhhbtd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/goumshekr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gmtmnlnli.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gqbzwgjbi.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gtkcymtai.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gauumoury.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gwzhdnhfm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gzvpmddaw.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gkctcrnay.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gehyyeyyt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/glxllytjt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gimzjdeif.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gbaukdiwx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gadoxuhse.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/grrrfcycv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gbeglhgxc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gcnufttam.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gwpewmloz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/guhtqkvtw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gkcxbnxez.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gabpstnkf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/grftqfnzl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gqikiwfkw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gwibrthbt.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/ghjoertwg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gpzzfufmk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghbbbtjpm.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/glptzapqg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzanlshhy.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gtzdqgifp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/girerhubj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gramccxax.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gbqcjduzu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gatbrjnvn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/grklkuabd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gzrhomjsd.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbkkjpvdy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gcnqgekws.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gbufzwipl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gticaaktu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gzehjpaep.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/grshdngpi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gcxxtxfqw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gzwrhgwwi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gzhwokilz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gwpmdtckv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gljwiklth.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gzexehpyd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gebshwhaa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/glichkyjg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ggfyivrtf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gnkeibidb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gzduylgpp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gkvpmpfsr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gjwgytlbr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gkmmytizc.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/grfurmhyz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gcxupcpor.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gmamsrsrp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gwviempqw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gsatbxacl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gdltashuj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/goxeywluv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gkemgoxbd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gpdrwpvtd.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gauwskuyi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gpgdekiza.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gygbcwwxu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gssigbrml.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbjoephwo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gzbfefrfx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gcoyggmfp.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxjsvvapq.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grakjmrrc.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gjjsqrqox.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggtvrnpmd.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/ggouywabu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtsnembch.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gefpzdgen.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gwxjnnvcw.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkcleqfuk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbdueolxe.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfsrjhsuw.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gblzonyjo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gaatxwata.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gwcplbfcz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gncilfyhd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gailpnhiy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gmndsxmzy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gnfxicamf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gigfohegg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gclvveycw.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gsduaxqxm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gyeacuehd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gxywoymuf.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gqmouqmbe.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gjnphnlbu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gycukhrwr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/giuriosbx.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gcxewenbq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gfldgylxc.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gebeyjptf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqpfmxobj.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gihapvpcv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/goxgzlais.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gtmmxvlfu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gtgzuahrp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gozawpmjm.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxhovvkmz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gcyfktjfy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gvfazhmki.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grscfgwcu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdbhmzsnn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gecgnthfe.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grpjubevg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/ggydrkyhb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gemdjlwbd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggvxhpxjd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggwidrqvh.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gnabbvytj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/guoqjanqz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glvlpvudp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggwnbyeok.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmkjsjptp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gebfvygut.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gxpbofgfz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ggltmdhzi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gunccdwny.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/ggqvmlgsn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gbujpiiom.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/guqixnawl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gluipqend.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gdnbfjyxu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gglwxaexo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gxepoipsk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/ghvgsfffp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gwwodfeqn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjcnowuld.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gslqscbhh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfomhiowi.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gkwkkjnlx.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gpqoauibm.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gukxiybms.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gtlxsmtxl.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/ggewxwwmy.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gmwkiszqg.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gyzdghczq.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gqqaxynnb.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gzzesawvw.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gxdliemhc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gzgeljjoa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gamdhkkzj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/goulqebjr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/ghdsgmpxf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gltdpdiqf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/glscrconb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/goehwcjro.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gedkaeldx.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/ghqjzrvzw.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gbacetbjv.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gwgfvughd.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gcottkjzd.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gitufzfvl.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gaeiqnspm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gvroxtqre.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gtwbxatao.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gcrvgzedp.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gsevbecze.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gsdvazqge.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ggqroodcm.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gtepsskqo.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/ghrhxfxda.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gslxsyqhp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gkcprjlap.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gcfyuqqma.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/genykppcq.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gjufkkpua.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/glliwsycf.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ggzoaugne.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gdidmzpnc.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gqygohsnt.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gzivsngvt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gbwzgfsrs.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gikmetepu.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gvwrsdoxa.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gslmsnkks.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gcjjfcxaj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gowdeleia.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gyqehplta.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gzmzkmjmk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gllcxordg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/giuewfdwb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gmgknbcok.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gldsmqwdc.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gzbhjdkrq.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gnqbylydx.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gafvanqho.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gvqnkqfuh.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gpxjmjdtz.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gfzdwwviw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gnyrezcut.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gkyrvpnew.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gwjmyzzuf.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gtampeisd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gkjofgvya.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gznreklbz.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gcsgidgmm.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gbqgoydvh.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gdrwbzeqp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gdhtjgfbs.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gvntjljvy.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gjwiempaf.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gphxzmgta.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gvosamjwr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gltnqjuvb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gcloxysur.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gcsouxumy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/ggjuotxpu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gmieeumwr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/glqsoaica.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/goydtrrxg.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/grdctohfd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gstyknzcf.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gljukvbel.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gdaiujqcw.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/geagbtbyr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/glskfrkvy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gjnswufyk.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxodohemn.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gswjjvzlq.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/ggerntiqs.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gkuyqyhgn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ggvmmwuhm.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gfrnybrzn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gvvctxgxy.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gpubwmjqz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/ggxluvndj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gkieoxafx.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gdhbswrcf.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gfekplbzm.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gxytqilhx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/grbsypvff.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/grvdddxwk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtwifngwr.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gdyrsqitx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gmoipksph.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gupbsacaa.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gsgzyhtmm.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gwunljzuc.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/ggqaleiww.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gtjhelyec.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/glmtikrlc.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/guwnljwrc.sHtML


<!-- 参考信息 -->