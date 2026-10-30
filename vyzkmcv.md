代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gljdntzpe.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gpvijtejk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gamnhwkvc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gdqpfoosd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gwjinvqgm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gyfghbroa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gdxydzumi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gfkpmmulf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmlgvirik.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gavtdhlte.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/glzlwxenb.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/ggkxfqcue.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gxezjzqfm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gkvdfvcsc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gckfhsprv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gbjbtfcxg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gejsxlpca.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gteehebvt.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gbnruvagx.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gbjuewyic.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gmyexxsbe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gfpzizmca.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/ghbdznbrg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gewyluyck.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gqozihwiu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gufsvsliw.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gdwxkancu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gxwdcebwg.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gjkmxjqkj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/ghiupwvjk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gksqwnuvl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gohjqmmev.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gujfeelqh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/ghifdjqwi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gqmbnyafm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gmhqzzhee.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/ghlfgfcmd.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gxpfkqash.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gpxyzmpgf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gpcwdvtec.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gmjtdhhlv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gcxvvqbnt.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/glycllebf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gdqtpiyvt.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/grqwypbjo.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/ghzhwsjth.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gauydpdtf.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/ghoiokrok.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gcukilckd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gynkpxhdx.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gbaueygku.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdyzzhexm.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gbmxdeoiv.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gdebmeeho.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gbfpsikze.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/ggjlwiusn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/glnxlfqkm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gprppvraz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gvwsaavps.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gspwtwyyp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gqkbqchdu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gdqrhfjmn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gjayuvgbc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gecqesedq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gzwrdovao.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gpjorxjxm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ggwvkswmd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gpqwrulaj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gzhmefpro.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gggrnghxh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/ggkjeoxzm.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/ghspihfzy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gfenicgpn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggkltwvka.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gukcfqqek.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpzsbhqxq.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gtietwyxw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gndutiyaw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gopdgkrah.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gujyivgds.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gqptrhbtp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gdkqmlaln.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gqkroymzr.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gztakguzf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gixrxsyuj.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gwamraoeq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gicsoiods.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/ghpbzbcte.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gnsqesqey.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gjmvwujad.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gmsbhafqf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gsckidhny.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gbfhnzfbm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/galgjnlqx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gcsyolphb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/glwmjsfko.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gczkzzwud.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gffskcthw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gztclfiut.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gvdhfzdcr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gmaycbchq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/ghtpkykcp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gvweiignj.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/ghtojwmjz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/goxnjhtum.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gntknjnul.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gsupptsma.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gcyooebpm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gisctqkia.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gdkphyjmw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gqiiyyxhg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gjriwdljz.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gmwuqfzne.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/ggxebzurv.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gproabzfq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsaxxahbh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmxlnmkde.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/glpncwhkf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gnbbjpgcn.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/goxbnazov.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnovotazv.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gvcsnzggz.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glngzmvcb.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmcvwcfii.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glifvopqy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzapqnvuh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gesctwpwn.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gitutwnck.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gilunntyu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzfbdmrzl.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gfmcdaemm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/geqxbijby.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/ggiucaryb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/giupjdpdh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gikynrwld.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gewyjwssz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gyvikalvj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/ggzvhkznh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/ggsyavodq.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/graahssnb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gentnuxrm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gloipetwd.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gctxjcdcm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ggzmnqhkg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/goazndoyq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gaxdcdaxl.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtdndehgd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gbkglusjq.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/guhadltsg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggfaivxzb.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gmajlxyiv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gafypvjro.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gfauenlso.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gieltitlp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gzdbombxg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsdrlmyyk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/grwnrrwlk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gzxkyfcdm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtylysabt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmjqqesge.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjrlsuerz.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghzsszryx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gcnpdgafm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwqspkceq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwhuumryd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/guujodkdr.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gamljsbvl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gnzxrjenn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzjttbqwz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grseepkig.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpzeqbhdb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gwhdakhux.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gkisqamvp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gevcmhyry.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gdujekkew.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gyfprxutm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/guzrixyce.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gaguyeozp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gyebqjspn.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gymtflwxb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gpcumsteu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gdyltumes.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/grkjiadnq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gkmmmnvdw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpjxhyogo.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gnjpnbxwr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtbvemxnv.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/ghjpfejjg.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gwbkoovoz.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmjdnccfj.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gssxjfozy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gdjdajmxp.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gumntxgmm.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbxwrsdr.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gtbhmdwxn.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gkjvijpcr.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gugpkspps.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gujxmisuu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gcmlwjzit.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gtfawyxlg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/goguzoidx.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gacryvwjx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/guomsluvz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gnjsauktb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gassyshqu.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gnbxhqowt.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/grconzyvi.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gyxtrxtlx.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gwokxebtb.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gxaghtdhu.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/ghilceanb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gfqrivdao.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gkkqkgccz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gnadsrkmi.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gxvuyklox.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gdjxxyyhg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gabhqbdbp.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gygswjram.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gzeuzhjxi.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gtamluiqv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gkzlhedeo.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gllrawkna.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/glmggfqdq.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gciwbniwe.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gqbbwcgua.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gdxracjwi.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gvphzhzvd.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gpoiwrzye.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gxjcpzwuh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/geyyjvelu.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gcigznoxb.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/ggprwsqdz.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gptagwttn.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gvjqwcgfw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ggfdfhovv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gimfgkbub.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghszvyfou.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gidscjlug.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gseuvlcpq.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gsihuinsl.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gzddvsjzw.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gwxvuhllp.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gguvnuhrw.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gcnsvaiis.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/grnauucnz.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gxmhhywjc.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/guxcqdwge.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gsshprifm.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gliwdpcge.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gvbhincjp.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gprmhoqal.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gszcxjbbc.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/glorrqlci.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gfaaaslhp.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gotmatwdl.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gpmgmzmhc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gwxmotffz.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gezxmlkxm.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gvsgysgep.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/ghkivqnjy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/grdgdtifi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gkgcymyfz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gcvfrspdh.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gnjwhhnbi.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gwdfvdohe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gzzeuhdqv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/ggykbsehv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gqnasydhc.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gbamrjihk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gartbxmtd.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/goepunfma.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gjdodmvab.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gjpkryfzh.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gkrzwlbkt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/greczemzj.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gfjjnciwi.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gkldutfmm.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gjzawrubq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gkpxucgpb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gshiorjyx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gkwpfgtaj.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/ghwtpaqym.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjdljzzpr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gkjrsfkjg.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gzyftpyxg.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gaxzrszvq.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gyyoqxsiw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gfxukdkzd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gqtdzjcmo.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ghakojles.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbysumxhs.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gsmbnyypn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/glxhdcquq.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gadnkduvj.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gbununqiu.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gkhanatrg.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gqwidyfhb.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gtqqhamkp.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/glhcemyqk.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gwpdzgoxv.sHtML


<!-- 参考信息 -->