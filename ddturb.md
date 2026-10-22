代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2eysasftk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xiniyeeb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ejgnhjzl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sdamiyah.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zilpjugu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ebhpmdbl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqgecydo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2czolketn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mareowoy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2iswcndxj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tkthtnri.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2evnquhcl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2luzmgrdi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2tfpzixlg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ypvsoqga.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2updxfkst.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nrynilct.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bghzqwpd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rciknhub.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rkengxek.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cpisopll.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2qoymauzt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2istlaogf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nstiqiby.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gndzxvpg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2mwssnxgf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xnhcbniw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2prtsjhpe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2hmandtbl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykofupue.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2awnehwkv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2sceghlpv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zmjdbcyu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rpxzscxw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2emtqddgd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jlxxjiqa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2wdbxplle.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lrqfupqm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gnvudugx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2abqyaqjt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2asikkhmp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ndfplylr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ndsllmuj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rnskchns.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nsjuzsoz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ftchmukb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fjaqjjsb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gsufixue.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zgmnjsuq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2rgqfelny.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tgamkgwz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2thkuqncj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pmjtkptt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fprzfsjn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qebqhxis.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kgukjrwg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2eqbsaibr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2bfgcgrxp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2tkuuzozl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gljwzmij.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2drurnepa.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2becfrlgm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vzbrpfkg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rzulcbfh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vbxfdagl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2yzsqycra.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jyzzgbnn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2lmtqzpmc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ckctjbce.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlcvvdar.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2otpgbqnc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fiywcpqp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivxbugkq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2koagxxqv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lrmzkmar.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kjmskngu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nzhtwqvi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ycedbxjn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2icveyqts.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cuxeavcl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bozbhmge.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2dvqzfupn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dpsuopwy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2omvxrqxg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2polsbbab.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eoywyodz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fpgzitnk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eiibksgo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bmbasnog.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gmklquvm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dmlryvfy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mynedgao.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cuqmjdpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emdjpaxo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2cgzbqmkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngvwhgoy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uitwwbyt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mfmimtmm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hhxjvdew.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2arbgagxo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2elesosmm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ugtsixfk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2nfawrznu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjgendzs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nwiuagex.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qbrrsumf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dixhxrkd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbtptkyv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2npznfsuo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mfhmpyoz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2noizvcib.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2otjblgju.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xdnmebeg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yiqcjncj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2osrjeddn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yrxhtktx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xdfmmspo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2avknhajg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rrderoac.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vmeubypp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fhygdmat.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wrmfrxli.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gfagimju.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ekgedoap.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rjntlhhw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2yjmnoscr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uhzmiufm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lagbdnmf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lpzafhtt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vchldece.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ewylysey.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2edmvdguu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xnqlxaex.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2npjznzeg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pazlgwwb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlsariet.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rctevnqm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dowdgdho.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fobgmvbo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mayymhol.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyxcfiog.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mpblgoll.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbgbkmhh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvplmvsw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqjbmprp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpisaodq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rripmzmb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2amacuhlf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tsyhdhuv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ctqtkdif.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2cfweukkf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yeojhjgl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2defjclpd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dstkgstw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2knvnktoe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zqxpnqgu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2drlnsdjk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2pgifjifn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zybgdotm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ufibvlgw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lfbqcjgo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2svhchxdh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ukelniqq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2soldhhmn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sywopwai.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hvqwhclk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ojnmtyeu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rswknroi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gnujqous.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flfzjmdy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ejbuslan.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mzgaoxpz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2okyqsziw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rwoulnjp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ymbvuwjt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ickhsrif.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dcyqbxtt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2vciutmlj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhrajgrf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oeibnsug.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fotbaznn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eyhgggrq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mhpkbenq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhzzlbrj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnxvhszy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwkcpaet.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ptjrxrcc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2swmkmcih.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rlmezhto.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gwfzwmoz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbhtgsvx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uxcyqtfa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2bdiytsrx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cigpzlni.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2eizdsdao.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ypojphxq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fygqanuj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hivlnkqt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cjwxklbl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aoykgnls.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yglujueq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2oymhbeqd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2xvunbhns.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gwujnmgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqmiebha.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2zudrzqoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qypskdfw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2bptjoxrv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fvpwsvlt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2twpdnmrb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2idwjbwcq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2pddkyfsu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tksuvduy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ldvyoqix.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wnbzruws.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmvmpeeu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2aaxklhgp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vvmuntts.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2awdotftm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfdyipeg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrbjzibt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggbnvtpn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vqgfmsnz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2cmixqdtk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xqrgizlj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fwaxgczf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ndppnjkj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ehmpmkwy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2oakpjdjw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cwbazpsb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kdxrhksl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qlwqtgpe.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ymboipwm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jyaiktkk.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lrmmfyyg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xjjuxpsn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2euvaxsbr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qwczzvdz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yghmwykq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiegcjdz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xvmalyam.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kcqgcass.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bkitrgqw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2scvghcyi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wdfqxkmb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nofytqhi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tzolkypq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyfcjtlf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kmjpwuue.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fsfugyfp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2erlanzim.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wglvcspp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2btvqdorn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xrtezpxb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdirgwlr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tnjhkarx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hbljvmdy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rqqtgaht.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2pzbvdydb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qqgvxwyk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pijddqrf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2nnudfcuq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xmeyeldd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xydgnesu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uafzdfey.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kowcntfb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hynxamfs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pblzqogq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wyygslez.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wnvghklz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2oqgzeolv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vwzlvksz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxwhpghp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2pvdpjlda.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2isyhsgus.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2cfwbelou.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ajtyojkk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2pukfsitl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdkylkep.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hnltjxwh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bmfhsiuw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbepsslc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gcldwpgv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2niaivjal.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2imppjcoz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2mjtamcpf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cwlqwuet.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2emxrlhvv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2olsljsdb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lkvhbkih.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2siizivus.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2lzqsuvof.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ffjzuyck.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2oauaenct.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2cavlrlpj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uquijgxd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2uauwyhnp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fbsbtdzi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2pfxojucq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oapssaxq.html


<!-- 参考信息 -->