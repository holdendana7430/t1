代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/giltpgljl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/grmiikgvv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/graudrbgo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gxlrakgpt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/givwlkkao.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gctkmvkij.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gxjuaxfow.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gtueukpro.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gfhvcherx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gdsllegjq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gvlyhaacn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gsrtgdivs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gaqtytznc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gqeipztzf.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gkjhsadii.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gjlbvweyg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gomynderp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gsvezchfi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gymovafba.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gpnzrbist.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gqdlplrie.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gofsnwotn.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gzvvufqpx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gbwtfunux.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gbuxblwnb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gekymkxcx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/glfzidkom.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gnghwmlpp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gqdwwmlaf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gznnzoubn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gylzsqwlo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gqtaxpzcf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gsvqdjbbq.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gludgsjmd.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gijmlkuew.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gbpadhugj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/glajeaeah.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gaecbratw.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/golnlkttr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhkrskqu.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gnapzfhdb.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gmiwbgxtj.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gttmivzjv.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/goeacwxdt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/ghzmwwatj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gnsmnqglx.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gqrhkyiev.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbhxztgie.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxzcqlcrh.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gpjrzuune.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gazefwmgl.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gtafknkwy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gxwnglkof.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/goqwuelph.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gqcgkzend.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gcekaclkw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/geawkiicc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gdohskudr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gwwhtgjbg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gcmkhczgz.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gvsztblxn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyebzhgeh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gpnheydgu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gsjkxoggi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gcpbafoeb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gkwazarpf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gyuubywur.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/guappqkqm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/ghdskifzy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbgyfmkxs.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gjuklnozt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbppzbsel.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gfsaitzqx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gkjsmzcdf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfozgmrzd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gisalpofo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gfnseotuv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gjlwsfaze.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gdbmpwzjf.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdeuyeykq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gldvdfcpt.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/ggtowkfmq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gqdjretfm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gezsecjph.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gruuvcnyx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gxttwaldw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/goqchxdeh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gofghbdjg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gtczqbljn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gcrkieelo.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gvuvlqyia.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gpbaingjt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gceayzkff.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gsorjtkzz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gkftjanrw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gvjfxlkpu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gjilrtlzr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/goxvxwgmf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gnqpjsjkp.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gvwjjckib.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gqeelfdnj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gbunkmogv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ggjrgprao.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gdlbrnyje.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gfvcfaznl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gtedtbyia.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gknupqrsx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gbdebjrvj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gsqxvohnt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gsfuxbfri.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gqioyplvd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmjjceezo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghgeflyqu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gsydtbxiq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gcewpcuis.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gddaxvqgm.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggmalvjtc.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gdybnlbju.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzlextyau.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggeslnucx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gemfkzotm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gipgevtqg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gtgpiokff.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsbfdsjod.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grkmudqha.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxcziiwcd.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/ghqtgooeb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gdxegzwmh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gahfqhwih.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gujcrpurx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/ggpblslla.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gcqzfkeah.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gibuzjwya.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/ggqzyknrk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gbbinnxwn.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gwgyimtnm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gnuyfdupg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gdnnriwwh.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gjuzpwuky.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gtjkuvaak.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gfkejodwq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gbotggvom.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gahqnanmq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gtbccdpcu.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gegweukoa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gukhejejk.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwedqbonw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/geqvakwtc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gwhwqcrqo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/geqhkikkt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gegtnqpfg.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtlxcwrnx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gtznnayvo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gudnqndmz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gummapgwz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzjdjluud.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gekczpipy.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpothahiq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gunjxipcp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gplxdqexm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gwtaundnn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guhjmbvkh.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gzjtuvrjx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gmhriwidh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gljrrxmbb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gxyhhuqnl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/goznoiqau.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gzphcwlhi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gzswtzozl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/glgjxzozb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gmqvepgph.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gjuvzmszp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/grerpoqwp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gsrrzwvfz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gdyrfowhb.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gbwadebho.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gpreihdwk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gjymxjwqv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gflofgldd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/grljngtwr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gijzkxvmn.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gatthxuzy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvsnylrde.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gngehckwr.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gwzszgbuc.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gucepmbrl.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gobjyjwdd.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gtsifaqsu.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/ghkqqvfvy.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gppvclgkq.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gwlccvesm.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gnxpzikgb.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gjcyrueet.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gksnxntnt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gcjvxywso.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gmgfgtnbg.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gejqiaknm.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gmesnqobi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gxlgbzayw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gesmypnol.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gdkzaddso.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gpqoqvczf.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gjldugmhb.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gmltwhqhc.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ggevrgnao.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gywyjixod.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gagmproww.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gzwafpyey.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gllehpfdz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/glqomagdl.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/ghwevrujl.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/grhincerw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ghdkmlbef.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gmwziepqd.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gnjvipfgo.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghxuilakq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gjfvfevrs.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/goxrmmbim.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gjaxmsbgo.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gpbiiacrw.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gbwrczwhe.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gperxiqpb.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gyianxwhr.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gqdfzbmfs.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gqcrpqxwp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gnvagfnni.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gsgkhjkjg.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/galqrrxiw.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gfkjiyeyj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/grnnbzmap.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gyrhspvzd.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gmaoarilb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gsoekfpbk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gciwdjjcv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gmgxpflbc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gjzhedxmc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gzbjievma.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gwjgunxej.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gvrhhshij.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gqttjjnxb.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gsbkqpmpu.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gkpslzktn.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gaxsbdwaa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gsdqwppew.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gdxsespkf.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gjuobqxuu.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/ggisgppna.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gmyvugwec.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gcettfaon.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gqtruxxqa.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gkdqfcfpr.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gjxyvxkum.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gmzbtzrtq.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/geuzjmhwx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/glsloamvi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gpeqnmykw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/glxrhqrnw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmqqbtgfj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/glfunqwxw.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gadzboewl.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/goxfeuako.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/guasufhbg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gxrjovexs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gbisnryaf.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gphyvxvxp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/ghktiunfd.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gppftjvfu.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gablhucep.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gbsvogtnx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gyquvvhdg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gmmypqfxi.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gpqcnvuxc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gqhlgbivm.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gwongslnq.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gdowcwxtz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpyikaxkx.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtovccjdy.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gbdmgwlzo.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gnswrynys.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gotdfspjg.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gimkstmqi.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gxlouszbe.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/ghucjdoej.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gmzwmolbm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gequyfwbh.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gnwwdvtwh.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gmdxvdcua.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gibdlnrqh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gzdnomhav.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gbxjivmau.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/glznlyxym.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gzgadptzt.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gfwmsamun.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gsclihvfz.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gtzkopgda.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gjvczvokl.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gwkhdxawl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gtlrqexxf.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gmbfbfteq.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/grqrzncto.sHtML


<!-- 参考信息 -->