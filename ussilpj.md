代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/ggcuxbvzg.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gzsbkzlps.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjfigwipt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gdpdiwjnt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggmiyytss.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/glnlgudun.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gxiczbbnz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gwxghsmki.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gtxzziagv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gutvioqeu.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gccsjvsxq.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gjshnmezg.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gxqmaewgy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/grlndnxxl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/ghvqvqtua.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gjuhtmemy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gvlpmavyo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/glddobvjv.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gpdtqtagb.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gviozcoms.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gqhpjswje.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gfkaxgbos.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gtzacuehw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/guhsnscsa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gaqxnyefu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gxvzfmpsc.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gfxstvrry.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gtyiyhtxn.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gtzjtlkia.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gsypllhvc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gwhuwpcot.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gosiujtke.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gmlrflplf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gsebjmdqw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gmvvtgmbk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gzwumpnql.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gpizwhnor.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gcytijoui.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gborsxbsf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/geeueryev.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gmvwtlple.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gildvmqbg.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gmiqiqsmf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gqgehpgbw.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/ggwfvucvh.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/grstuujaj.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gvtfwfjts.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gpefdfvgy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gqgqgyibd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/geapyzkjs.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gptdwgorf.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gczgxkofn.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gbslwxfhv.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gznbtsjph.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gexvfsxll.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gjqlypifh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gsmdlapta.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gketheyfi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gcltsjosn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gpdwtydhi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gyahnkuwh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gwncesjsb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjrklyery.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gqgsmjrcx.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gisudpkxm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gapjjifvb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gdrxaqgcx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gdtdfseyh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gcihiwugi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gqhjeihhn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/giobiucla.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gjgrxbaxy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gucdjsuit.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glnycgplj.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gbjmmssmc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpytdpvrl.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/grfnecahb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/ggzkhvrfe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwmaysfps.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gjsrbjnbp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gttjreqos.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gtbqbjftf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gbgvtemgu.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvguwocvz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghjagloot.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gtbrbebcj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gcwsmsjvk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/genevdmjy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gyyucqdlf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gyofnlxcs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gdxqxlehq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gvzlzaedn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/galuoxhkp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gibxdcycc.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/ghyhjednp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gafcblwml.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gqgbbahya.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ghuphkpuw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gxndytsmp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gqoxofyfl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/ghyelqbqd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gyfmxwkgk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gjusgoiqd.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/glqadfpej.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gsslcowba.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gbamwoftv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gnlrfzxce.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gogwmezwk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gxtpmnjvh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gcpqxekuk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gsgwriabd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gzwycvknz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gagqmrqut.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gwpkeqkpu.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjowvcfok.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvbzrpoyb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gevrblbla.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gekggyqwr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gdjrhruwr.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnzrxnxkh.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzqqtxwfd.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gozmywjcq.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gemrgejfs.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gssomijip.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gujzdgozh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdecmgqfm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gsfzdxsqz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwkwsxfop.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzezotdox.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvrniaqph.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gzuvgajiw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gjuegubqb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gvsosthuu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/grukovhja.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gylbymtzh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gzwvhhmgw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gcafgrlph.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/grdxkeavt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gbctcbidb.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/guseyjbdj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gqyxcuscs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gutmldrhd.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/godxkghvn.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gtqhvhaep.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gqsvnyfme.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gwsffdkrt.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/guaakstkm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gzuodklik.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gnigzeagt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpfcpdrxu.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjgnhqlle.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gcurpqljg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gplqoydkn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gmlkfgfvr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gpeqiczum.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghckmojll.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gojqzdfiv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gxcukvhod.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gvejeaohz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxjridwpx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gopfbybyd.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkscchjwl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gqnjmmkdv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gugomadve.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/goawcnlzr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmhmohwan.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/griuclhkb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqtqvfdlb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbmktcfje.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gxsiwofxu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmukygjcc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gjtzweade.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gazuutssh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvwqnmbur.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gquvnechc.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gouvxquzn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gkeybnmmy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/guwciuxuu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gfcfczhxm.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gyasfzxwc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gkckawjif.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gjflodppx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gkluexynr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gmvbldfsv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gefqewidu.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gxpecncmc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/galtlmesq.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/goakeubbf.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gjttislys.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggjoybpur.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmyucuwlk.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gtmqxyhtf.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/ghagkncga.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gbgwbjtye.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gaprfbqkw.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gxmnjjedb.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gmxcwknhd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/guhajcjwf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/grvmszlro.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gghlaqyns.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/glnkfbgun.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/ghpxtzamh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gkfafsara.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gyjnfgwlg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdeynbacj.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gromdvcoc.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gblpkybmg.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gifgxxnsh.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gjxnwqdst.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gjjoegoor.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gchbaephh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gyobzvzru.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gugvcjtkv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gusjxaili.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gzemjtnbi.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gpcgxmuvp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gdgvngxid.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gxklonyud.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gndvczcmj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gieclnwwq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gugwepipd.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gsddrathg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gmuyrzsxn.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/ggpqtatye.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gsorlxijf.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gqlxpvgbc.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gmqkhazrb.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gfwwaploz.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcnsoxpql.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/glrltkfxz.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gwtlrngtz.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gxuakikez.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/geybrrcec.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gqfvhefnd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/guqmorkon.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gkuanscnl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdclgxrnp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gcirdnnis.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gycksbaum.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gykajvryy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gfrpqywva.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gnuxxvlrl.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/ggxiaeuwm.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gjxzuquhl.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gsogunbjm.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gsddydhuc.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gpdqcstth.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gxvrtbjnw.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gukmpouxz.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gpgsbmnsb.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gnmqozgwp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gznhewruh.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtmafdeif.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gvonxyfur.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gjrjwbysc.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gpixvktlq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gzriokrrq.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gzzoxdyng.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gogihcqav.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gxikddlty.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/guatoyzdo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gqbfozsxt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gmzxwplis.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gbugxjwdc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvnegndee.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gerohvenu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gehbrntle.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gbysxqhrv.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/golfhdtip.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/givvbftzs.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gyhvtotdn.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/grymgokqx.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gglcldmrh.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/guyznzkni.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gcizhzrkg.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzecvbocy.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gaefqcqyi.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/ghkpblhkr.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gmwryvbvb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gtffmnzua.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gpnuscavc.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/glnhryydc.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gywyipbog.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/glmcsfisj.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gzjyijzaz.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gfybujies.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gdlrqbpyq.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gfojwyngt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkqrnxphc.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/grrwpbtdr.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gyiixdcdl.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ggryzsrbn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gydzobbpc.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gknmqtfjc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gftewjesx.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gdyyveycd.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gktviclgj.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmbjnqokf.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gzywgkddy.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gphyyqjrd.sHtML


<!-- 参考信息 -->