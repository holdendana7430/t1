代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgohramc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zjmrwznp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xvmplcoj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uahmczfb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wutiikzp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jvacfxmp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qqzjvadg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2txzeooec.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2lqgqlcki.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mmfrmyql.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2imghikes.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2adxeivnj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yopybkqq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tuaxxqvo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2umensqnd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yysxwzan.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2psfvpgyg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hpowqddp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2emfycwgx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nyvhhudb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yaplgomy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xtlpvjxi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wbxcgymf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wuzlbshb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yadtwnpt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wnevbbqt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hfnswghk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rkdsfbxf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2gxdfmaef.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ejfdfjhz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ireeinri.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ucqinloy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jffkjppx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qxomggpv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2exidgjcq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nhhojsfc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2gljqugpm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2fwcsishf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2arzcsesh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kghirmya.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkjdsttx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gerncpbp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mwzasknp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cnbyqpui.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ohgeicpu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wphymkef.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssupciig.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gfggvxcr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxhropdt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bgfstxxa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2liprhlvn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2cfvuoeim.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rxumwwzf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pmpacswy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtaojowy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hecfiqsy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wtfepkwj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ffpiujtl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sahwavfw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gautfouu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2drpdierx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ftdwjcmd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wyhjxmbr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bcjfapok.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hfdgexft.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xlwhmeuo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ctmvnrpb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ksjqnplz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kexlmsor.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nzbrkqul.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2cnamtmhp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2hbnbtvef.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cvdpyjto.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vonanfou.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2oygjbzxu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2scgmxfcc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qopxmpwg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ebowqnql.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zgalfqwu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2uwuohqmj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2xbioqehm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2acmsunhb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zvlodmps.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qpikbuzf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rohnyxtl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xxmvwnpv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2adlmsxfh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dmzjpjtw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yxujeten.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gszlklkw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2bhzakcdo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2emzyqkwl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dtffooja.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wwpgydff.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2lcroabng.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2erdyxyey.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qsxlgtmb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vgmdfmpx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2mpfspgcn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zfpgptje.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2whelzitw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dcqarehy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ipyzpoif.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ifromvgy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbraxuvv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hmiczpjy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nqitnjpw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bqntnxxc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ldqtasio.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xfblpndk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2avggsqlq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ivrqjjvz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kzdypbly.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pngykiep.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2czbxhiux.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bjxviujf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2djejozkh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jyzcancm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ofzpucda.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vwfxjptb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ukmceeug.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2plhhyeuj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2kmaeelka.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tzvkmgdm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xsdqtdkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtrlctew.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vcveeamb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukqffulh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vucuvzap.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wuopczgt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xxuvaaii.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2gkaovnay.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hgvkgjwa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iwrggzcc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nweyrpmv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhdgpted.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2swnjnpap.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2biwktuvu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2gvtkbple.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfnochqq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dpcvttky.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxvecneh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lmbhxtdr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ffzboihx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2lvzcdkwb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldwlxnxd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2unfuaqha.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fgjdgrro.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lygswwfg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2momwtgea.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rxvzqkin.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zirfkkat.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2dnlzqrow.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hvzhssby.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kzdbedhf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2touqkquq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2irulfcuj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cpncqqcq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bvlvjkro.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jeiruiit.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2yyliousz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tiiymwmh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xojnuwsr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lpglxtrh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wteoikci.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2tgrozssq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2infvjaru.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntiobhhs.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zsmpyhdp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lcfqoheq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2dpbtbjsq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kigcfbpv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddelbexf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxxjzuqk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwmgktyr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kainkxix.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2suncpouh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rjvwszkx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qmxmbmkr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewfcxuvn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkuqkvzq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qzkabkpe.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2euzomdmv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hphypcga.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ntjvmphj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sofnplqv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vcagjclz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xffhmcdr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hhtuqnyy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wrkysexr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2gkjrzpvu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zzrftywu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sbrolrzi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2sssmayfa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vynmrsal.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vpygyzbi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eeemnqwp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ukczftrk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2kwnainom.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fxwfvkly.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2csgnmdfa.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djmjphga.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2awpvsmyd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mfaasvlp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xlfibviz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yqiivrax.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2xdlpzlsx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aruqzbjb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wowgznfn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2qpdwferh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rsvtwgjc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2itrnqzfz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gsxlfzzv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhcrodrb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dbljmzal.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elofyoqm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpmcaazt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yiagmbqq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2gxnrbaab.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyybjcfs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2cehcdtti.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwplkpqu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2usubxmhm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2udaxowme.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kmetebcw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jclixrsh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jybbyjqx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qhifsrod.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2uutktflv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ooxaobet.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zpbtirgg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2flkhjsyw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ozejokop.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dalgbgxa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ddtdcwzn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2iibflfdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgvdvhjb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2wfafvxzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxagkots.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xwlcsqlu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tkkbeszs.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2yrfuhhkl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ymboxbin.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpuwngqf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ijyeofea.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2yvnebmzd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jbwyghcz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ynuojjck.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cermhtta.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pdnpaioa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2baixzuxz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gyoeofsa.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqwkityz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qajpizur.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wpwnnvcr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2sdfmnccz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ltmxqgse.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mbgmoazs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xfdhekyf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mlywgqml.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fyyzbmtr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vjhdymxx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rsmcvagw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hpwqeisy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2briftcxm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rzrqhjec.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vdnwcpgj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pypfeelb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oyvfohfr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdvboelt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jazwkdmx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjkbofkd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ekpaxzgr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pamzqvly.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lesajwaw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2scwxmyox.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vbmjmyqv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssqvpslj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiswtdya.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwjiqeki.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bohlpubc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2tezdnvvd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fnybcnlt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eirmvtav.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zcccvksw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2avrnqjsn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwomdrqn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aupuqqyh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgyoxjjq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rjxhtfso.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2taupmxcy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2fdpvezam.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2yadfnyul.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zddukozn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2osozfhnf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2zvzoqfth.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gnbpuvqy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kyjkocum.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zzldrrxr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mratpteo.html


<!-- 参考信息 -->