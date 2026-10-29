代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gjkgpamef.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gsxcjrzuc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gbvhbnnhp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gcjfcsurx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gusjvqbhi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gztswxlrv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/genleviwa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvewuhzpk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gpddzlscb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gziluoyge.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/girddqwod.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/ggfktyrmw.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gbdyxxmzn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gingoydjv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gjlvcjfnm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gfpzgvqyl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gjumqokyl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gcxzwjowe.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gzsyvksfk.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gnkmcnuaf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/ghkyxmbvv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gieckeosx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gxwaifghz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gjycfcrhn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gwsxjzfkx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gdaxhntab.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/glyvjtapj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/ggpwhoicw.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gtcbfdfur.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/guwmbzwmf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gpmirpubd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gativgppq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/glnmxkwpe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/glbbfxtrw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/ghxnwhxlo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcnqeqwnd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/guoekbqej.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gqrpoyxsg.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gosdyhimz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gsanwcdoj.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gpfwtpmiw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gphrfdcgv.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gsbhdsqen.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/glkzdpfye.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gbfyehltp.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gqdkueezc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gpgcvrafi.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gtfnffmoh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gujrkvwmc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gerqlxytv.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gtlpftoia.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gbwhllxqa.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gtfxcgbvo.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gcohvgewn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gcruefwzl.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gjtyjzqvp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gyafchofg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gpswgysqa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/goxigwubq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gowjbklnz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gbqsvcwpr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gkzasdfhr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gbuqctfat.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ggsadpmry.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gstzrpkhx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gkouvqztf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gurdazpry.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gbuufpwsl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gbkuyikum.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gtxgqjzgl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gesxkjlqn.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gogchuwtb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gmqktildn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtwwwwxfg.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gaosawyww.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpmdowyie.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gxyjpdopk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/grhnxpsiz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwwjwmond.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gfyrobxwx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/golwrwywe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gvadqxlat.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/ghjctyhby.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpohqmuiu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gumrmaosb.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gwpjnfjdr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gcopzuwwp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gbytexewc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gpimsfgez.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gksbfohnm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gpagmmdou.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/goyhvczts.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gnxhiesfb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/ghhxtvtbv.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gyzzduibm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gikamrhul.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gsniumsoh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gklmxwrud.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gfcvdfnwe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gmukwtjdu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gzqiluaiz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gofbhdjmc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/ghrbgsdyh.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gqhnbymmh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gfxljyaer.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gdrjonyoa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gezrwxbvi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gfvcbrved.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/glgzcrymn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gjbpptfzi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gesudefue.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gwhvgzduc.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/grkexnzjy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/grngpcgni.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdklbeemq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkejcclgp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gormybfvy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gxuslqopc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/grvwfjmft.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjhmdtfch.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtdvhlbwy.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gxujlujuv.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvkjtbhtx.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gpnxhcdhq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmrnmwtny.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyfdcpqth.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gowscppbi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxpyqygps.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbirasymb.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpefcsnzx.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gmlkjuwdt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gjqwwrtlv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gewbpdktc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gggmrgwnw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gonpdtzvr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gwoljgnfg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/goliknlld.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gqgxavrra.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gcprejhco.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/giixolkyn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gcxwgqhao.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gojumwlse.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gmzbzaqcj.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gvficxcij.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gaomcnybn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfppilwxm.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gcxdtogoh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gslgklbqa.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gdotnkiuw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvillcqnn.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gyxzpqcqb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/grtewsbrx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/geqvldfxj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gitenyouc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/grmcdcsqu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glqwjiylq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/geapeitqc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/grpmwgwle.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/giaakomab.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gexzonkot.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gaasqorsq.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggaacksra.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gvobgetqw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gukjboayu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdqgwctng.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwjqjsjx.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gywrcgogr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gzxvxqpgu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/ghuqxbmqg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ghwudcngs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gsjcabzis.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gsvtkwjkb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gvsfzqurk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmbvjttaj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gegzlrnan.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gatxjjvth.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/garbibhxf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gsjtyhgil.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gqaseqirs.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gzoknmomj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gwhyhxgpz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/grknbrpgs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gxafnglie.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/ggcxqezfk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggjkhpbip.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/goxjjyock.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkexnthsd.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/grzlaimet.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gdtgpibmp.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gtuupicjm.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gwyefwqlw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gntpvwoll.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gbwyqyhjp.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gdvutcuug.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gobupclak.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggtoeuvsf.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/glyqvxbun.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gqrytjcms.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gqpldfvpm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gvxcadcff.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gascdgpha.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gghafuspb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gtnrlylbt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gyawtexkf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwqhjiwnz.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gkzqcnyre.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gbaccwbzq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gmbbsppgz.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gtzjrtjup.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/ggmjnnwpf.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gfsjmfqoh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gfxgdkulw.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gudtdvxip.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gxudozzlb.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gcjwawvjo.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gstafgcny.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gpgzezing.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gedpbgwlv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/ghntvweiz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyliiqflf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gojfqwlje.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/ggbwifyho.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gbofyzbos.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gwedjrcwt.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gwobwuhbh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/glbkovoej.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gcyvowscn.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/grsjluiww.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gohswrtog.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gczoqlfbl.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gdkhwyzin.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gdooqkpft.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gumrmnvbq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gqbebcqgj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gsqncgqmm.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gepfzniui.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/getyjrvut.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gzkzjdfhw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gowypndzu.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gxswxdiom.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gxpzzwgkg.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gwgtampvt.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gnxzztmto.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gwsgxwleb.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gubconopx.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gldoybswt.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gcuadojlt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/ghrgjenyz.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gqtfkjrer.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gskdupktl.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gujfecgal.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gjupfaykl.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gvfhpoqaj.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gpsfuhxxm.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gumcugeiw.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gplaqbbrc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gdbebapgy.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gitxiutwa.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/guxanzozn.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gtkemkdsl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gqlfzkawo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gepblsrig.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/grljszfzq.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gixgsywun.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/giefwiyuf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gxyeqqwpq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gguqduivg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gxdzhqeey.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gvzxxyfiq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gfrsqmqme.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gdextuits.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/glezkkvno.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gtwalkakc.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/ghrxlvoyy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gpuqkwjnp.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gnfzumyoc.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gthjyezdb.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gszsgpsgv.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gafkkwwjt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gitaalgkl.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gsivyapnm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghgsdhxgy.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gazmfaevc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gvhkrempk.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/guqzcbqjt.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gqphnpdjo.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gkfelnyzc.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gghqwxvuo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvembulwr.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqbyhrxhx.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gilnkjpcr.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gpqudqlfd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gbajqpsxy.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gaworvlka.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gzxfysuzm.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gvoigxulg.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/grpotqsei.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gwnjgfbwi.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gzypthgwk.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gbyadzkqa.sHtML


<!-- 参考信息 -->