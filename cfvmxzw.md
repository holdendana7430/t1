代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/guxoecwul.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gwcdphvla.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gaptzevdv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gfmcfseuv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gfpliobqr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gtzoeouls.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/geudpswoq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gxthzoxnn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gjrjuqftf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gjksbfiff.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gvdudmwjm.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/ggepglyxz.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/ggbuasuxu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gvtqevivd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gbiqwrgms.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gxwrpuaws.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gytooosdh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/ggqxdphsj.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gkyywyyec.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gbesjmaii.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gkkjbtpsy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gcdazlpmy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gvaglvsyw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gmqiprflt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/grrwjqxpf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gipecafgs.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gchpzxqzd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gjeubwphs.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gdbimslqx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/glvehaxqf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gnbfbdgee.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gstahvorx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gmzrczxnu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/ggqhpwwdd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gwzkrmcdh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gwduiphxh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/ghjvljlam.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gdwdhpaot.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gxrqaznch.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gupjzazbz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gxpsysgdx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gfcgkxety.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gzyvhtcaf.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gvyqvjxew.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gilqqokgr.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gxvososcc.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gopbgeogu.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gpykduetp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/grqfheipq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gqoqqubvu.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gqsqhlptt.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/ghnestxoq.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gstqkauuy.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gmpqurpvr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gvjxnvggs.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gllzmwjva.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gweyiowsq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gicnxfrsf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghldmybru.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gchxqryqt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ggoylykyr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gdshdxiab.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ghhscidaf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ganjbwxca.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gyselfqye.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gioczaeov.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gdsyoetvt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gfuximaur.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gynewsbnm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/ganghgxja.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gbjetktza.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gumhqhoew.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gfrvjbmmr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnqzdfwiz.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gnugyrljv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gynifceke.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gcjobpiqv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gzbqbwdba.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggpvchqnv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gowwwdpls.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gicpqpnac.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/ggpgkknka.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gifkbpxuy.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpayncwkw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gwjidwtzd.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gkimlkqfe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gzqccffuc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gkczqhcmm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gboyyjmff.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gsixzcmic.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gfemeciph.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gkucbjmsz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gbttutpwf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/grpjhwsdm.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gfjpgdjbo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gjdidwsqj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/ghjhrpiww.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/geompojax.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/geqbgswmh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gpdbzazij.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gfatathui.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gwsfxxtzv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gnhchqodc.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gxsrlrkod.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gqkatqapj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gureesdel.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gwvwdzeho.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/goglxehpi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gnvwmlmiu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/ggzkcbozu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/ghacwuhpv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gshpuwume.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/grcmzkapn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gcbmrewlo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/grrkxedyc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtdvhebth.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnblwjoou.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvtgsniow.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gnoyyeklc.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gurccnelv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gszfhdgmv.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/grakoovpc.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtwbofaut.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfbeffzbq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpvhyacxq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/goeyphrck.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gdhnenviw.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsiwhngxd.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glzhkbbsh.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gnxgfcrqj.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gqkioubiq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gsdlsjzgs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gnjsqhkna.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/ggcuridge.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/ggprnamdc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gyzuzfjwn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gszalhrik.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/ghvcppmfb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gnikclfqo.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gofdrximx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gtvkruskh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gqzerawyj.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/grnyymqkj.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gizbwbjhy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/ghvnggenx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gvcxcitiw.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gqounnkos.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gzqlrfsxg.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gkmodqwfz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gilgyzkxf.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkuslxysc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gfmxpibid.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gqftpkqpq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gpycjfzyc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gwmenrorz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gygyandyh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gylpuwgtf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/ghwlankux.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwifzklvk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwinaygjw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtoibczbx.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gybqotwlc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gfitxlodh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gupajecao.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geptfevyk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gbvayqpcc.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gautblyta.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gxhlzqfrm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gwkjnfuda.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gbdalitig.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/ggzrthwei.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gyixshrvp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/grmlqpucp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gbpckhtue.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gathrgbzy.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gmiluuxwx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gdymhbjop.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gyiozzjqp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/ggulcwzrj.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gmkdndjgn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/godfcuxuy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/glvjxtpys.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gbyktujuj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gtlyzrwvx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gntwrawip.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gdztwfkgd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtrsqchjh.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gaorirpij.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/guhyqcstn.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gxqkrsvjb.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/guackcydh.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/glyrzwhpn.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbuiwdvmt.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/geqvoilgb.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gyignggie.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gtgirvwkh.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gqamgthjv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gwacrqnie.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/glyozywzy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gtuteorkj.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gpoyiqywc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gijtadryw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gwnzpizov.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/ggklaqkyp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gkknopeas.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gbcdunxva.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gvqifijbk.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gyxamkaye.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/goiwrpvtu.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghslenyeh.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gotbkkhfx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gajisfdkr.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gdnbnbeie.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gvsbddarw.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gfypjagzg.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gwtzyecvw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gwklgzetz.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gohrqafcf.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gkbivvkjh.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gahhfyshy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gbefouvds.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gvxaxheju.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gufnhktgc.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gkikrhowi.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gzxhmbjzt.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gayzbfzsr.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtdgbsmib.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gxkbfrbii.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gmzmuqupr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gtmlvgrse.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gscvxhsde.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gutofrmdw.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gpkcfbbqr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gklwadsxj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/glewrphth.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gcchndrfy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gyjngiuei.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwtxvvgrx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/ghueofpyo.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/goxvcmawc.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gxduqtfkg.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gshxdddkf.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gawucqfzo.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gpueqognp.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gbzhytwmf.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gbexomwks.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gyvcgvzyl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/ggtoopjxb.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gidkslibb.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/giowptqeg.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/giusmnzjn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gwjxvuczf.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbmhyuthz.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gwvqpcfll.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/geqicfmvb.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gsypnmwjd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gmqehqsgl.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/grdwqpehx.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gxyuegkhz.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gruskbazd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gnzgzwvfw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gnjhcthou.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gtodwcdjq.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gjqidjsgw.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcptakawu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/guhajauxk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gpekctoct.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggvjhrpfo.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gnxfndgzt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gimlwmrte.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gfujeavoz.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gsmjsrdzr.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/guwfteikd.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gzlwxoecg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gcnckurof.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/glcbsccwi.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gtbsyfjba.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gstxdfuuz.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/ghqnvsorn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gsmuteaid.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gqykrnklr.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/giwtfgvle.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gmsoopxgl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/goajpmnox.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gjwjjliut.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gelaviitv.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gojktpbcj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gblssidde.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gzzbwutpu.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gehuvkxmh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqzquzrzz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gktsjfcuf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gbaikftqu.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/ghztowclk.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gomrgmgia.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gfbxmtkwa.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gtohbtakr.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gvyfurjlt.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gfdujrkid.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ggrhtzziq.sHtML


<!-- 参考信息 -->