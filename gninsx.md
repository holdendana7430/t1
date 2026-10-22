代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zoqraolm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tjkswnnx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pcelonbm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ggmajuqi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tnvxtsso.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2dnesjokv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hysydvgb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kcevmbuf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gfgbektx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vppheozt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fvkltiod.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ttdqkknk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bxrijirt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hkzinmxy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zvpvwclq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zletuagr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lddfjsjv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xqueoizi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ntxwyymm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2himwwqbs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mhjoimjg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2digurqub.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2irsyubbn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2aoanvxcv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2brtnruao.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hprkapwi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lgfexnxg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ddurdlsu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2srvbgwje.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rwcogcqv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qnilzpbt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ypilkrlv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cshkufan.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ctuocfek.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zkhifnig.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2lujdbpbr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xsjozxsr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uocibkpp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jbtlwfhl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2brfchlxe.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2znsgiwxg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdfyptdg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2paieezfl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2huxvwqbr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxkfthhs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kjqapzwy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2udvlqago.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yicrhajw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pfvobtrz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2nbrtmjjm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2tkznlpwd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2mvwyyorq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mqhuugyn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kljrnvpk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jkulpmlh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2eoowglgl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gydqcppy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2uvycltuo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2remepdgw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmngrunf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ttpmuocq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2oasxkedw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vorjitlb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2woeasygi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wumhdulx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kzzpraxz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qlvvssra.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2aqgoeltn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yfzmpxjq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sxqetieg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ssnekhog.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ziffdate.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2banrpzjc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oljsihua.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2dtadnvhp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2eptbyolu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2baiokylp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vsalwsfs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xyhcpndp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2awkvawkw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wphanxsu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bejhyslx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2icqvlrjt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ggnlrnaa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2jbdazfvm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2frffznmf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2hepmeutu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bxisznin.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vdalzoaf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bengzpvk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cwilovpz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2rhalnlsk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ifsdfyxu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ndywadbe.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2yrayrcof.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ptbvxeni.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rxymulax.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xgupyxdy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vhwfraly.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jcmknpkk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mwhbarvm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zyfnpodw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2awqnyifr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xbwgrriw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2brzppnie.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xgoangrl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2libgfisx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zsjvnwgf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xeikmhwj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2qdupjoij.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2georqpfw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uetppyco.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vhijigvi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ctlduyqi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lfxsnkhr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gxbhvpum.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jqwovqct.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jaejqnao.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iqxjjjmg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tdchcjxh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lbtfdvwb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gkkehrly.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2exkcoltf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fnpszmjv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rhjuwmfh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hdxqwuxb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2znvxpcpr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jzplvmju.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wajofhpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekwnlmbt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2oebmncfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmvjipyk.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bcjycpaf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bkeubefy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mgeluxsj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2esuvcjaq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tdtzftgp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2crwtzmdi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wqjkhpyq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrilrgwc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ocdjcmpd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxvlsdna.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gdgutjcd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cadwhcpt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pptblkqo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fwgvilav.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bryraqsw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bsazezui.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2joubgrrs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpifwovi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ehcsnaig.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sqsekecn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ohedsyqu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mgkhcels.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2chkwxnkh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2aawjhqjs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cdgzwykx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lcrxjyzz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sscgzfek.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vxxnszjq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mnfsojuc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ivvsokpt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2htkkqynb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iysxmqsw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lqynviam.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gvhdynvb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zlsswabi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2mwckhxsf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2upbgycdc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bridtzqu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mfedqfug.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nyzlwqey.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjqvdgxr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ovzucyhc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ebpjdlyz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uzmswzzf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pstbjfxy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cuafkhbf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qohoztby.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ordyesye.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmaxdaly.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbxwesbe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cioicars.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2womiwgqx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvzyvilr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lgxvvtva.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nptxpuuk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xupiqduj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fxyrgzwe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ksstsmte.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tbjkxtrq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2emwixrjy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2dnmlzcty.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2owoqsyzo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2uvrwxmmv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rxbqrexn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hvpavped.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2lnbrebdt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ydofwyhu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mstveihm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yjjufpjv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bqwifjeg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2popgdezo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2bgjwsazw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ngkgcppq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2novtilxm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rjthnmcl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tvvhneqk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uhwdgywc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mxpyayri.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jmzsdyfz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dyitapwp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2akjckudv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qqgrkbzj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tkkatjwv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fkahsdxw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yprmxtrl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2emowpwig.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2yaidgwdp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snmgabwe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzxrbagl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uuaduest.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dplhjxsu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djdjsdsg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nczpeyoj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcoraedz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ucsagsaw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jxwzqacs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mqfwgbxk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2shjoevax.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2njxviczu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2spqtlroo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2muumujvs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vlfeffrn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pfjqigbf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gqnibkuq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2koqnpefi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hntplvic.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2diwnhtth.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2bpsdrizm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akzqvnea.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dkpmznaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcniywbn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mwaitigr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ouglretf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyzklnub.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ztidsalk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bltkmnoq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2iwwxcwss.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xhvaiauu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rrjhdcxb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyuuyuxp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdwcaqrj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2intgwtzt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2tsdfzdkh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvnzoawv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpsrllsv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pegvkbbu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ntxdabkf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lxwqkqhd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2racvnpww.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nesttenq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rgupmewa.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vnlevikn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2werwmnkq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2znhadrqy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2yopmbxor.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vjebbhhe.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gwctuaxv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ejzmsyuu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2pifusvai.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2slfggytj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kenimxex.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lmdpqcan.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxukiilf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfiazirx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sgyitibe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jqbbesyd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jrgyxtbq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2msepslkh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2kkzuejpx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dkqtydkc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zosjxcmk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kvscidwo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2aejcuhrx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2raojyaor.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2apolhtsx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jcumstqs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2frsstzes.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jgbqtnqc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeoekfwr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dfrsuceu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqmtzuvn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2exzvbecu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2iuacvwdd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2nduiupab.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2cukhltzn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2cmshxxfy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cvrrwnjf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2umkqyhrj.html


<!-- 参考信息 -->