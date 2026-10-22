代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ourvjtrb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bhbwpujr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2njlwxtdr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cbxwmsli.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zqvlapko.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2iunywavu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ovkzxwuo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ghgqtztz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cxyhqiuw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2abrnhzyt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jowtwqtk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ofxwjlpd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2svdvyrvs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nxxvgfha.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xvzdjavo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vlloqgfl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2gznocpmn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2slmqmaem.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ljcpgnwy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2oqesmxon.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hwkwhlvx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pcehufnd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uxzeqsty.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2blkmmbvi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qmpteugr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gywiypgx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ilweigrw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ykrrpfpl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2jxmrkdve.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hhtbbjmc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ydmpzjvc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2sotrnwpe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qumoteva.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rkskzjcv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2npcyufsb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2enwzvdir.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2pzccxcak.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgaoklgv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvmcagfo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ehgyvgfg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcjochjy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fnocsseo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vcbkvytm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyaahmqm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2twrpsjnm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2pfelzvbx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hocpemms.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2anoajvsv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2adwhavjj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dnhpfneo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2efspbetl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wsgbyztc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2aoswmsnx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vxzoxfnw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ormzyjvt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gfnyknvk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2reekiumv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hbljkrux.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2lflynhjf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2anzjotia.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbfvcjog.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uziturgs.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cdgzaolc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hovbphwx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2nosjeqph.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ijjgyaer.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cncbqait.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yhyqjmpp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2onubgess.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2yfcmpqhg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hbmahkuo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gmblfcgm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vlufvbjv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbfeqqeu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2udlvyuhz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2odyofvyh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwzexowc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2phhcijum.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kdgsmjto.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2rjlclwew.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yaepkoat.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2eadnptli.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ockkxick.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uylclrnm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tuwcanue.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bkscsmdk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xoffrhmq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lejwsgmp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jxzjinbn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mpbvnvle.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wnohjblc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vfgcuirf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gmwoqbxn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bxnsvxif.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wygnyxjg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aeikudqo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2dhyculcl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ayelnczs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wvaxuspo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ceqmsplh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2txrzjjuc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aeuyeote.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jcwfmclq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lpoiyorz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlfzpucx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mevophzu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkrpvhqg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2mjfojenu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ymvkznir.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zknodbsn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ygnqtmuv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ppnmbstm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gazijacn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jhmmpzjm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rkjssidl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dnmaokxn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hquwmljk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbqhaykv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dvjpudeq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lcvvzzox.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ffrxuoww.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ogvtxtou.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ojqhkkwv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tjfqcslt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2idjimeaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blmwtdkv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2irnfreal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2futujbxv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfqdikhe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2foookjpi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fsawmmpv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dfpcjehh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vjcrjhic.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dzumlqng.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zmtgwcfr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypqabnmp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zynqbwju.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gzgenony.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dmuwzhgv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2llstlrlm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2esfkgahf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzbgchyl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yuztzltx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kaylblwe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qsrdfsrv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksodqill.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hqjlcers.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2pxlkznjj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vinenard.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aupskylg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2sdzznuhb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zbehphoa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2emrckvvp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rzeqstsl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oghkfzme.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2kyxvsjci.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wjyehant.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2lqaohbzw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dzvzpauz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2menjwcaw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2kbftwkfc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xdjogwqe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2zmnyijzn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uilrojmb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2eqikrtkx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2oejejvpc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wfxeeonz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ecblwtwr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avdcxgsf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aoqksooj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zytvgbhh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tchsuywz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idcnmgig.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2claqqqtj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfbzklfg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vomypzlq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fajcmrdg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvmilgnj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2egbrsczs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvmpqfap.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwsmoria.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fqrrhkfd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hjcuvxqd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mglpzceo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2znagntyf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2iwjmomxd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yqsvjnzz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2auselvcu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jovffdnd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zhddbsxz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lrrhzurn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2cxpjrnzh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ttimqsbg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2afncanpa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yyrnnjff.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jumxktmo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gpsauhmm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oxcfqvyl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iuxnjoii.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fvqpvmtz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ltzctzls.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecoeumlm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zhyathio.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cgourrno.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ubyclhht.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xguadfuz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kckwyutu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lcizfegf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ctzbeoro.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2flwjvdbp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmzrjwxa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aqxqkyxw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dwookhda.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pnzynsbd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2lpmtquam.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rqsywqkp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mxuxtjpt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oubimdey.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrpbnevi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2htlgeluq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jybtfzhq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2biagvmqj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2shpvovgw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2eggqkkqb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vnvjsnlb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjegpcyp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2iovcvqbz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2segxeead.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ziayyxvq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fcfnfizm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hplidijm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ccmusvne.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2erdrnfht.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ymsndtcf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2phtdofey.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kbyrbreq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atrwuzdp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2crnkqwvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cugmymvp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2cwasdchh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2cpjjumhi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecqzczft.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gglbqtxx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpjvylre.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2oknyglrm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cxsnimbg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2iyuhhkxt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfnzsjbj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ppyhiubg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2gnociufp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zihynyxz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ejloilel.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vilclixm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2plqsphsf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pvzzhlay.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zwdnqrxz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvkpooyb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qyobtflz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ndxyzgwb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pdjmeapk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wxsjomwo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rdympqde.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hkeepmnf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rrlrmxgt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yolpxjhq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2zvelogfx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2lizhgzqr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zxuesfgp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shjldyuw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zoaexvkb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uymhwlgx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ibhqtoqv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2txwciivw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xknrgrtb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2iudxcyft.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2spiewija.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2javopcer.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftiorxgk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uixywxyf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2heeaxipj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2octjucfn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wzlsmjdc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2unepgvpc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2daypzdbb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qvsylzyr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2aagwqoqd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iccvezug.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyuqhuof.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdwjwlgj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tgorqcxp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ckndchgb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2urvhsjdn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2yoivupkm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jirgubya.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2fnsdsemr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gxzcaouy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lbxgjxyv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ywmmpttp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ayzksiuf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ocmpqzcn.html


<!-- 参考信息 -->