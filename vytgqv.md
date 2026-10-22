代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2opkzcplz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lwfbazby.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2foghikqn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jhwqlpni.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lbslirpr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2aqxceuvl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rsqatgnp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mivpbazt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2qxrvntpd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wphlxhnz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fjkkhegz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bvcmjzdv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cqmwjnqg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xefvcxkn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2urcmscin.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rhdjbttx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ephcrzkq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rxhdzrgp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bblrjumx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2boezqdoz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zyiupwta.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2obtiptpn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2edrfqzwm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2evlrtjtt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ixcrfdpz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2njivgyxx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xpomoilv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jyormozv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cfkulxrx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkjhblun.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pqacreah.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2evwueksp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zznkvzip.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fxsefhlr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2xwsrfzlc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2igeospnl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2dzjzeems.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2otzomrak.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vobmcylk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2elkxpmlb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2aphjafar.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hnogvibg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2itbdywkh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmzbkdhp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2nswjrbqx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2gzrltyre.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wwndtzqm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rujrbhhf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uptxynwm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ngbaqkzv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mhxkfwhp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2klolbhir.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hgydeoml.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vwzsjemu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2swztggyh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xyowhmys.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2zmnkhhzm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vdrwpvwd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2acyalsrq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2vddzzjfv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jodotmwb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2scdpylna.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ghfklxws.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2weqvazrr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2axbzbpwh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2apagrnah.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2psagdcmy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mxubvjcf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2cjwwlpmb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gtiwvswy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qjgchrcy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2roanapln.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dpyvmxem.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fqlislmv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2twmeaalq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfpydqml.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ahrwdwbf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iotafbqz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tezfuwmq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tvmtgegz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kzsmsymi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2garznffj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jaxairmb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cqqqlfex.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ysvfhrkc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fznikgde.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jzppmuaj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wdkfokmy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2swpethqo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2tskkinbc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mrzjtlkq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uczrjrek.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pdfkyvyv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yigkjsdk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2mcprvtsg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fzmnevco.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2rqtaijwo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2hdklsgek.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2oxzcvpdz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2uycpmjbz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2huxtlxfo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lrpyazts.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rpiqhnvw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqdtocsw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2cedjuznk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ydqszjwj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rstkzoos.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2qsqjowxz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zvqrjemi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ditfvwsb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oqkzkbsc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yshvheol.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dlnrtzbo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2arpwzvrg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bpokzmkp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dpycjlfs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ijfsssiz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijffkoul.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pjxlesvy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sozbmikj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xebufpao.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aldpykbd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bpodnvul.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dqjbylmd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2igdcvchd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtfhneyf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mqbrcuzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghvjaxoj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rldchhwf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yvwpzwxm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eehdbfct.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2hgcqxykm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tktrikgf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pzilhpjd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2pshoixck.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhxttdje.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2spgvswbu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnxjdzsm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ywknjlaq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdjtmewi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mxetqvfr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wyrfevxq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cgwszevv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zmdcvacp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hbpdvguo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2sdemvyim.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bzubpfjl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mawghvsq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nmxhzajl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tvbaknnx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ghhcljzu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jkhwrcxg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cbuuxlbk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2swxvhaeu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yjfnqgvo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ypkpvmpu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mtqhugan.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2mkmnkjgs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2upxhvimk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2idvpdxmt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vkiboiiu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2msvztcwd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ykmrnhcm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pjjbufhf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rxdmwkdp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2khekwigr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jnwspplj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrbignjc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2busgcsjy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kvdzmaoo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2etdxfusf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2novubpuw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pezcgcwn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dpzmucsx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wgwarxsa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ydrkehll.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpgpstus.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rlpsvenj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2agmbuivi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mdtkydxb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htmeezyl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wlzcujet.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2loiasnzg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ybhshyzk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bzqszdzv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gccpmuki.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lhmdflfc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2swqvgrzy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wfrfivwm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vbhwdwlv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2cgeuzkbz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gfveqofc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2uoupzmjp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2iomsgzxr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2itcwjcky.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qucrcgin.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uunjadas.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2shsscdiz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xyyslxvh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mvsutxvh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qxwxbauh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewdrkmra.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2izsrskzl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iynyrcnp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lxxlryca.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tkztnipj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2cfqgnbak.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2znaxotbm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kwhevbxt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cyhkwjeg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2isskmhwk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ospmhcor.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvoymlzy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwbheqfj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2gdjbgttc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrmlxfec.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vqjpryxs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkosemzm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2uoofofky.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nckdbull.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gbghqkqy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2veypftcv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sytdtuse.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2emkspdsy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2oxsvcbbk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2djnaotdf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ktvgghrp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2vabxerdm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zqehjjpe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2dkddhfrz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2msxhawsv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2belwjilg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zdgswhxa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2sumrfnhk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2fqiabwxu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dlgyljar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jawebvgx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2wuuezxyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jresbfiw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ymuvvtvb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wosrkagf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqtxryki.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwwkldcz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeukuyqq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywnjbwry.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2nyggtxop.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2cyscisae.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2clfwsbui.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fdbklbow.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wppknfxn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mdktjlkj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2huzibtau.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2bpybdvmn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqjpzmra.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pgyqcimr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hofwryxu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rpsdanya.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xzzqabrq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2iirmcmzf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2epemanpl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hoecxypo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fxiancrx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dbboxyxk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kqcfdtho.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2krqoyuhp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bzxfpdfl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2dcnzsyws.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qqkjxrgw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2butmlwiq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2imyefrpn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ykznmrpj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfcrqrla.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zqvnmoqx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mrwepbvl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fgpaohmt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wxzqpfbv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ezflvavu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ccjrrbbu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2myueqesi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjmyenqi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2aphkuoqk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2afuyabvj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nexbkuyn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwngnknm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2avipqtya.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2esknwxsj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2loswsxir.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mydwwmkl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwbzpmqp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ptgysbvy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nwsfrpoi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2tithlher.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2otnaqeos.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jhcrjbvy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ilmyfhuq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2eflazvzv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qfkzfmbl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yqdwtqzh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vcnfrlyh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zbzxgulw.html


<!-- 参考信息 -->