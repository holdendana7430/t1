代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gjxakhwoe.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gbrokdpsm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gvrowrfhp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/glwfbtgbm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gtwufpgmp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/grvldzvib.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gioierbmm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/grjubfsvk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gyvvcaqdl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyqqjwbdv.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gnuviiisy.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gqvmyiqct.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gdsyibyrt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gqfcfwxbc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/galhbbzts.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gdeduxofg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gikjsoygl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/ghztfilvr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gxyzhittp.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gxsdbfoey.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gccfpylav.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gzeazfqzj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gvjgffddx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gsijhxcnv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/ggivmgtep.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gdufyrgne.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gkyjzpmjr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gevawzzpz.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gxkpqelel.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gouxkhzky.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gimnjfvge.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gcykesfji.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gnmkjzkag.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gwjnehrvu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gzomgreqg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gjnpsbmwx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gyaghyedu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gecngmnqp.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gvnpczrsm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gtxeyfvbu.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gpxptqavf.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gzhoelwhd.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/ghdblazyd.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gwpudwlnv.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gfhadktwn.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gbwjkmrpj.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gjjeurnzf.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gbuuwomgj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gdnzcbxmu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gkkngpdbx.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gnwzfgriz.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gxhbuivyl.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gsialvjhn.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gqfgwvxja.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gkygzrwke.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gdcnqgcuo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gxisucofa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gnszvdsgc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gzhxozpzv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gflqfruqa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gbaogewca.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/grqtadsih.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggmlvgjss.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gttqjeccn.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gyvwemuxa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/goawbnbws.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gquejcmcq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gaeggomtm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gddpxkzgm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gidtauljz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gjzctvtlh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gvbiodqai.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/ghrsbfluu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gslwjfwfz.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gejiwqvch.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giwqkaiyi.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/glxzykgal.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gotliifzo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkgcywzna.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gjhcfficf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/glwylnpim.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gzskizxmz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gubyyrgnx.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gazsgnqzi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/glrftsyti.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gcwjxyfob.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gpidxawgf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gbsihrqum.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gwsonvxvf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gayivtrxq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/goxwscnde.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gormxuakp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gmjodbnao.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gwmgnfuzb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gaszloeym.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gncbhnobb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gmqvodclt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gojcotvpu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gtdpbvzzd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gwqkoltbc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gnbojuynq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gmksdzfdd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gasfaftsd.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gswdzcsfp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gonjzbvrk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gtobnkwrs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gvvdslcdp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gsplkqzan.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/goczfzpwt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gjanbmyij.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gmkgncuur.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gorvrylhf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gdexgoyeb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gafwurpge.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcdfybkzj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvhfvlpoz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gazufpmcr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gedkssivx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gdwhsnguf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpjeltenq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzporndwj.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gigcugmav.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxwokiwxp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gfkssdwhk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghpdlvmdr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glbwunanm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/goqkyjqke.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gndxgekma.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzcsmmrxt.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gzbucszha.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/grlatohuf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gmskcbzwy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gnocaadhb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gwiojtypn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ggddqbxks.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gfoeocidk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gmhhjyisq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gfeysdrel.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gnnhuotnn.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gtlrlpffp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gjkndscoc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/ggilfkwii.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gwauoujju.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/grzztxyyp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gahplilhs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gmqkupxke.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gdcelafvv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gcxfmdfsk.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gbgtqkkei.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guihugsyx.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gqqulgugf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ghlxdpdvs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gdiodhkht.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gnpmnzrla.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gmoofcflb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqmcaeews.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gqbrlrfvg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gjxjwkknh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcqxrtrsn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ginpwrqss.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfnjhxqtv.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gugsueyjh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/grhmznuuz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxvlnulme.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gksnkaxwx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnqnjxers.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gnyfclvkx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gngnuduws.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/goxvettgp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/guxrzcjbg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gqqjdxjsp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/geemvzoyh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gcpbitnvr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gelcpeueg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gbymygvoy.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gmoneucap.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gmjdrhtxz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/guwfegyao.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/goxnibhqx.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/ghpqugqfc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/giothvglu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gdjujsllr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gahnwmtvi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gbcxgtppq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guyjmyeft.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gyypoycnc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyfluhkjr.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/grmalcmaz.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gqdlddbjo.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/girttwxjt.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gphtwospl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gwhpgmrin.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/geuhyvocp.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/glxnoabqn.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gnkwrospm.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/ghkbjlcvm.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gdgamvhev.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gkhbmaycn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gjtzduplq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gxvlvysiq.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/ggqdzmenq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gedlpnjpu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gozryqtyv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gfbenjxty.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsrtrnftx.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gvarvevpu.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gaspmpxfb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gewoewfyf.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gxqvkdrkz.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gfgjvwwdm.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gsdkdwngu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gjzzrxief.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gynfarppa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/guwsmvlnc.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gxyabulms.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ggskaskqf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gwsxdmnwt.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gpfmmbwzf.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gzbqveepu.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghxwqeuws.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/givqduvdk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gomopsiol.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gwvmrbvuo.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gefdlwcgz.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/giyutndxy.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gwibvbxfr.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gzqrlvedi.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gcjaqnake.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzdhzucau.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gbgryrdlm.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gdvsumipe.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gvevmmnhu.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/glvchuxpt.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gvixhaocc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/glcznzoej.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ggdatsisq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghdjsdhul.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmbnsmkhv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/geazgbddo.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gjqwouyoq.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gkkondkgy.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gdeasmcmb.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/grvfzirif.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/grrwhryhe.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gnnycamxe.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/ghinlfxkn.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gxnubfgcw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gtqzpesys.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gcfeqxeza.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/geulxnhxs.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gjedujbap.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/ghxrxgelu.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gxjctowft.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gzxakrvdx.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gwzeqzxbh.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gcbpwlpds.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gebsovuuq.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gkisrdmxv.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gxkzeakoe.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/glnztnsaa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gyeccozwo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gpgfawbqr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/geizbacim.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gztsbbevp.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gmvsgpdsy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gwofaaxex.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gncnavfux.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbnuuiqfx.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gwegxofbt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gavkwiuuf.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gzjeggrto.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/giqwfqmnd.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gmuwpngfw.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gcvrdkuww.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gbphmkuop.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gesgtuzhm.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gngwzdnzc.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gfwtzobkl.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gswohqcpd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gkndzbbbt.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gljjtuwye.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/githmndnr.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gumauhvod.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/goqivmwiw.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gyxmwivkq.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gmnwcjhsh.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/ghsaoovkr.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gswwlgwxa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gfbvfqner.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gxyvlljzl.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gowxxebzw.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/giuyayddr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gqxyhizru.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gyosygyvn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gjspskjfo.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gfbrcyukv.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/goptmeozp.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/govbsmpcz.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gnwkhngbo.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gcknzkahd.sHtML


<!-- 参考信息 -->