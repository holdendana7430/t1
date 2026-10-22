代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jnfukrtt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pqhlgrdj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2oubgoqwa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rmtpudpi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajugqyzz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ueiiqrpd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sporgzwt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2khihkeot.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fqdoqexg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fkssjcvr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xmimvefg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vduoffqi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ssrigyps.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zslqlwyb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2lnhvoqzz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pllvmkgj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ebqnwcpa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2loieebzu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sxqiaxca.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fsaerogn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2kyrgeisk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2oxbaczns.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ltxnxibi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lnkubcni.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dwsrwzzl.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gcsvwvsk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eyzodtva.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2infnbgxo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2elbbhldj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bujsyskp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dvenjhty.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jscvazkw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tulcbzcl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvacsdrb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cpnrvxbe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cyoxqsbh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kvgrjodg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hwjlstff.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rqxvlueh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yazwowyv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2rivrlvmi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vseepaxc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rakippjz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2corptlbg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufliexcb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2weskhdin.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hmkwonqo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yuoksxkc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zmxzhjgj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zosxrwmn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2szhnlwvu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tvwokeui.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fhkiyxyf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dzvrnvba.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fxauapbf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2uuxkudor.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sfoqspkc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2awnozytl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qokgyrra.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ibnvyxle.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wsxqutmi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ydlrsims.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ferqkowh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mdllyoul.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2reeybkml.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xgjyhldb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nparaqmn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pkntyqqq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kwlwildh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cfmwsbvi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uazxlrrh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hkgxhknn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xeqylunt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2faavwloa.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2slfixsqv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2floyxrmn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2lsoftxav.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hgbyucxa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vwjeegeq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijucjanc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hosfixfh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2acvgeoqh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2eumyzsqo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2prautomo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2aldwrhrb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2xtinqxzg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nuureddj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oinmioqn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ivmwxcqq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cfoccpac.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vtxffdxh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2fudkzgpp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ykxrhcdv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dowyivww.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2idhvpaxk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wovhyort.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nbmdapgc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tvimxyld.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wtxtjphj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ffaifgwz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qmhtzgup.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vanogzlb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2xmivfkib.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ostyuetv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2uoojepyk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwjnnhjx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ekhbsnur.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqdlizdh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ascaqynm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ycvsjpni.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dorilruh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2usbuzwsc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2usoxgmlm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2grifyedc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sxyeuusb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2guzzfspb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qxwuabwh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2unmqrvfk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jkqacidv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ezitsezq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ysihesje.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2acfuoyqx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hjlqfvxk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kkjrzscg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rtlnzrpv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kvfifotc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qkzdocin.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2quhmhxgi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nylbdsnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gerhqwle.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rtxejism.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejgvvrtc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwfnhjbe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wfhubplh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pmhhxfsf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2sgrvjocy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wbzfmvih.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nztpyrww.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2doybeofh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2crmtbmam.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lpxrgvxl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ioybuwje.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ciwglzru.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfzsdsbp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gojdbdzp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jhfmdrel.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hxlxwbdm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fwmmmyxs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2wdmbuoqm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hwbiwrti.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xomfenvi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mcwbassg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2egzonimj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dwtxsmnn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wrrjfscd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2vnxoltyt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2usfwecee.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jftecptf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pcdoorpi.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmgkcnmc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rjqpfndt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2knoziuul.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2luydngld.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dtpqzgbg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fmefxfkq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qfqscmvk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2krvoabiv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gciyedxa.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sidzhzcl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2mvcexqtq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cyfvzpne.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pnubvjay.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qurnfsfn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zhwxegyt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2dtgaqvdw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmjbnizv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qdttmrcn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2krghzaig.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvuudlib.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wrdoxxcg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2allbxaro.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2moiheqdu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bevmmnps.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2busynjpn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnquspfs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ooixmish.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fzawjsob.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fzgfjuga.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nxljtlsi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xfsicawc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mibjqqrr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vofcisef.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hjjmoubp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2nummeajg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xrqtmsdd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2raafezwk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wkyllrtx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2iehhlmdt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pzcbfkfl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2krvovnod.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lddyzctq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qkoyvdib.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rkputmpa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2seawnitw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wzvjtvwx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eojohisb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lvdtirpj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2onfzsout.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tjjuykes.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vgatcmmf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2thtpfrrn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hatlgkle.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dmdfdiax.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ujuhraom.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtohluzy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eqlopfhw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xshmloxk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmsyzbrz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qnqseqfi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2saesgvhf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yucwsxee.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jolzbhhh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ouplscny.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhyyxxor.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2decducqe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpsvwtva.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfrlilvv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nwubgntv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qlefvcmw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2angtbugz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2czsymwth.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2uhmcchwu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2hbrqxhrh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2yxurumyy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zwevszay.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lkcugazp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2vzosfbxc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2fgzcxmsc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tgrzbmiy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2uuawtjtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brkfkbks.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gkpsfteq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnsegbzo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2eglspwnk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gdebyppy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2hifqfucb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nzbjnokt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mxfvcvnw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qtpasiwf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2nsvnsffr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gdwlkvyr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqgdcqzt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hyzflsks.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2lmhsoezf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qbowljhj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2imxlsoov.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zamfpmqo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxczadla.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kjaddtas.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2duhonlps.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzxrtgtd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ekdtrbbg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pimqmbdu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jzwoaqaj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2utezftdc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jdtoksur.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2gkxyibdp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hppmniuc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2prztttum.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vuifylhi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mmeqdwqi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qqedsgfd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2beqqeejb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czpryezp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfxctjzx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fitafliq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wgqiufmc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vxqkbvuc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2myzkesvz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2oirfymgt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bavnvoix.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxhjnzng.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2thpkpyew.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsyjcoac.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wonrrqsq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nkagtypi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2noekftsb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2tdefhaev.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2nlulhiin.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2mptdvykj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tipcllkf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2usdxfxho.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2knqauege.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yegldhdz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tuodcaba.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fdiwtvmx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kuhqcpba.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wlyxhhzm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zgcnqgeo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ayfsblrf.html


<!-- 参考信息 -->