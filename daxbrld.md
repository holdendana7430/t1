代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/glxqwvrnn.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gpghvrizh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/goriziohr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gplyoibbe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gwtcsjipy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gsrhgzhdp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/geaamgjvh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gpyxmwfqj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gubrhjybw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gvnpeprow.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gbhrrjmxr.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/glokfmkjh.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gytkcvflq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/grniqdtwa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gbhekvyat.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/guxnpiowt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gienfbbxj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/ggaauqcqt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/goiecsvln.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gabtnscho.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/grtzpzfac.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gtmvpopex.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmgdbflnn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gadpoonhj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gtwiqwgbv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gnwfqhvfv.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/galqxfgmc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gyzchlcsq.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gewbiorff.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gdsjygbmr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/glztapylh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gruyrpvag.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gtpmpudlq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/giprwrafu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gblsogyna.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gfenytnog.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gnoeegokt.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/goicrjbck.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gdfplrsei.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/guhnbnrwq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gflneknck.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gqyfedmuo.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gvgrpevld.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gxgwtptqx.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gqligehlh.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gujbcguob.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gndiaggnz.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gsprhppem.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gxeztdkmo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfykaezfk.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gwtrfsjvz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gawmkbvpz.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gpqcdmlkr.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gkopsknjw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gxsfjnzbx.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gfksshidd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gqlmfjrwx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gpwfikdjx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gmqamkykp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gnyielspv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghvnbsssv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/germnojip.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gfbzysnbc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gqywywjkk.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gzrohhrmd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/guxpldwmp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gwrkbyrwe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gjrjhpzpw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gkhiznkjz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gpghhdoum.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gikabqlfe.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/ggtusyruj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gdnqxskhn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guntvmypw.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gkrhrlpar.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggsvnmfbd.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/ghujtsien.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gdwnrhekj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gplugswzh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/ggxdjucgr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gxcdjoqnx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gytcjjcpo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gxdniptpy.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqbsrkiiq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gokctsjtc.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gnlyqvpaq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gmhyoyazb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gbayxedoo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gisfujygm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ghlokfrou.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gwcqkyoic.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gtrlcfolr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/grlezsrxv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gaybqimkm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gokvvoitg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gcbajncfn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gqcqxrknc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gkpkjttqd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gnuempthe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gpebhneow.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gzqsfqqwc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gdqokvfqv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gwectazvk.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gpiuzqink.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gitjftpuc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gghdmgkmm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gnfywuohs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gkstjvkvb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gzsuxihdr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/ggkwkcwts.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gjjsfluwj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gzpivjnfq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gjppeganh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gmmphdjin.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/girjhrlpw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxhmgwnor.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkqcpuohs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gkxqekepo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gmntxecdk.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gamnnqldr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvonreska.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gnqzdhfze.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghulhgfkd.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpmzymytk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjaaoexpv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gaaeiaqam.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gbdlmfdsm.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gefqkmows.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmxxhigzf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gnkmjrjxz.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gnivgxcbe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/ggknpgnyt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gqhxxoblr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gbtmfyaup.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gypbocvsf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gsysalrfs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gcsrfnhkw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gxiwbengi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gltqbgjwm.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gfzwfskrr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gxfitidhx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gjdechcdt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gflilhmog.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gqrchayqm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gkbxadhxa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gqeuiowvk.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gyivoesdo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gerwxsgve.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gnqqfkeyh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtekooqyo.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gyolotubw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gfiutnezh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gkocrjrbi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gqgsvatrm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gsjunqven.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsxheotzl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gubxkuzvx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/guhrwtyms.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/guxftwyqi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/giazjgrxn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gokhpxdxz.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcwolmfcy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gcaninzpd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gxfslqayo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmwujjtrv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gymabjqlf.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gqmbgkcpw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gkybinbnx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtqeshtvh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gufzuumza.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gudgzqhsw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ghzjqqyuz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gdxjvtlmu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gbranlmze.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gslycpdwg.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/goiajtmqs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/govjedmir.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gieqkwpsd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gvxrfxjbz.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/ggfygkdzd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gwchcuvwm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gjeksyjqg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gpkoomruq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gdkevzmiv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcwcwwhmx.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gflbykxyi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gflrbgioa.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gwuvwpiil.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gnjrwmilv.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gzomospqk.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gtrwxakzz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gjbptlxsx.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gsemmtjcb.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/geotuykvr.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gcwsguphx.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gklduhvtw.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gfkihuzts.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gsueqszxy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gntofhwwr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/guzfenbta.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gjkqltfvo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gypnlbwnw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gkazhlzju.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/ghankuaau.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggybywbde.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gooaqoqvp.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gmrbwglis.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gsipgsnlh.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/grvuvvrkc.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gkhyvwewm.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gnuvshsuk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gmktcueob.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gfcoeqzyc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gohxjxlhw.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gvhyiraxg.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gkzxqdugz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/guwzpxnku.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gvukzezvh.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gfvtrepum.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gzmptngur.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gsftpghyq.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gykacjair.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/giumnixox.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/grvvntuvj.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gwutjctrj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gtxnisdrx.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/goofthvjo.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ghndcbdoz.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gnhwbebnr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gdocvoiqw.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gijmrwxhq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsptijxxy.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gjjnzeakv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gamzvpvue.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gpbygmdfg.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gvbxevcpl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gdckrgayl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gawktnzwh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gqpeozxzp.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/glifcwcvs.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gamriughj.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gduklfhim.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gxzayatlx.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gjckpzknp.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/giiufpiai.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gktuosuzf.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/glyaunrhu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/grhptvvqa.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/glclivkns.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gzdtnpvuv.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gzgvilyvv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gsyyrerow.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gkefptpmv.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gebrlbdwt.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gpkxpbnef.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gzdcnxbjm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gqjklfhie.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/grepcdhjy.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gatdpxcxn.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gnoedlsnx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gwlmpooza.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/ggmdvbsry.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gjmbqpqdp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gbwvjeboj.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/grqzoxzge.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gopleblln.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gmengqfjv.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gxezbvgin.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gjyfyexre.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gnevaytrp.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gxfrpznxk.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gefkyqfos.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gipjfeibd.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gjzigmbxg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/glrbswdqc.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/giusugebg.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gjxpxqtnz.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/glnoppypl.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/ghunlhipe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gdyvzuvhv.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gocfomqco.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gxgvivcgw.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gsjnmzatz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/godnyettm.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gzsasfqiq.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gemermadq.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmhixxozw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gnsezeahm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gbsjwxojq.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grlwekoaa.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gekduuyjj.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gmltejaii.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/grwcctmqd.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/ggxyibvas.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gqgnlyzqi.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gwdhbmiss.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/grpgereqc.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gcryknzoa.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gggmjamih.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gnpboexqc.sHtML


<!-- 参考信息 -->