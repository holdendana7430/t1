代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dvibmcmv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mokplivl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fqiuvjro.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gvivgpmy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pixilots.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lrradxbm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xcuddtrn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2itfeiubn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2doijuwub.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2piwpkihs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2esybtxdk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzzwryr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2neiaayxq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ybtlogvx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bzqbiaaj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2whnoljyg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2qbtkbrdh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jyaxxsnf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ybctaztt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2njohisyf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ynwvlktf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zycmzdhl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qegdnjiy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ujmlvccs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2siprlzxv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jqqlxicp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rrhftsys.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jfcnamvx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ibffleji.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ydfwwsbf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hmiwumrk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hlwtachn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ecepiybn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qrdpnkiv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kepiqksh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wobghdjw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2flamrufy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2seokgsex.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xdhlazwb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tcnonatr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2loepbshq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ymzafmid.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2svermywe.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zewedurl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xkcbwmuu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zpulhkek.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2amkcgsyv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eiozcdtp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qjkwoutz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2aagcszkg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2obqjuitg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mvrwealt.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qfkxzpnc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2oepdzcmw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2woxgapgh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2lxcnigmr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2rrzauoor.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ydtkjvcj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2hcconqrz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zqkgjfnc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jnqtepox.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2pgcqwzvo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2neeufnjt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cezlbnmh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2izpmisvv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wzvftkhe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fjejfmae.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxlibpwk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ngjdxbxe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kjdcoxxw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dsnpezvl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wqlrblar.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iximsqjg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ioohifyw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hiudnppl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2keszlmru.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nfgazfyw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gttevmkl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2cdfglmom.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2uhfndhpt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2deufviir.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2tyuieogj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qkugxzbm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mlglcsmi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwuxldgh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iiqongdg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ajgdewyt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sfulqkpm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2uvmtunlz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sztmurfk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dsljirnw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gipdujhs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bmdkhlou.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jpmotifk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2kummnppu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2asukbarq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2pafvgtev.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zgruiwji.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2csmssvtg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ipfqwpdt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rndyrtnj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ekrsfxxm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2oagbmhnb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fnspbtgj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yiqcxfvd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ynonfrul.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tjzlokvr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wdsfydnz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2onrysarq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2emlygtsn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzpdlks.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ayympdgk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hwoaxowc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ecklinym.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2oupjimcl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zbsjitcd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2radfcbwt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yjbfbjxr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zyncxwkv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gyiqnnfa.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ttyuwife.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2zvedygcf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2hruudjio.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2culcwqnd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wsnvfpax.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2azmwcrzb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2fgclacxa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzkrlsdw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lndcnrev.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bcevvlaj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmvipllf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ukwxlnfs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2kwgbqloq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2whapasqm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sfrnlpzp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hkerkrtd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2stkknvlp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rksrbake.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bhriowfp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mvtipmon.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2elecokll.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjrtkfrp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mymkcfey.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ixjympww.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nzccczuf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gtwgaktl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hzszwgmr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vsoqzmxn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mkebttdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhxuvvgd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ewrbbvry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gatgemfa.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2notoyypz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rzutespf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uoccsczl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nwurmycm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lqslufco.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sjbfwclb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2uwhqdoml.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhngbsgx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gdakummk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdddcofn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2krppmcsz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ryfzxlqa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djwkgnrz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipyzkrni.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jqlldpak.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zdpnmtkx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2yzaddpoj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gukwozxh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qepjrebm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nscsggie.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ktiydnxd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ayzfrscy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uieulvxv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pnjzqmgk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gxvvspcn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qbbegwwo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wujvsozo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qkimwiur.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2guyxvunq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gngmxkbc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bznvjxdj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vvmbtvqy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mxhopbaf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eryhtliu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wyaywdjp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wixtuotg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nuwudbqh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vfkwyerx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eibmyyen.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xiiarfzi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llcdlvvn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xhwoekyt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wyrnjvwh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fleklpgl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thrqbifl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xhoahynr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bdumzgga.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2huwkwxai.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdghjrvs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xhbwlrum.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ejqkkxhy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhqbqkee.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcgckjnw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mybkfkiw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hogqmwqd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cwjnmphj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ghxkjlfw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2prcyklti.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zryvoxxx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zsiywcqc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vpnjydzt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2snrlwhhl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wyydhznv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qqbynjzw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rwfjleug.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndhgcvwg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gmgmrois.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qvwfoqlu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pkbilumb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ddcfzgws.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2oawhaqmv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qpvlusux.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ujmdjiao.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qqonavuw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nlbotnqq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sfusvsnq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jsvmidar.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nmhzebzg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2qroqetmh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gyxbaahi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hzicopcb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xkcatkgf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rscrlzsw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bnvvwotm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bzseacmj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ynqqzczx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2iojpmxgm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhvzdzym.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvfakxhg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jxymdmti.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhgfzssi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eidfowzl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pwozbmde.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgggbvxo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdrtiyls.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uxsrjmyg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2opzhwsof.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qudiwbyd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rsuazntv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qrrxegkf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2apqmprfo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2nhytbwde.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2detfexoi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2sjesjpar.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2irsvuifz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xguvfnxu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2lthmazcw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2atxpspqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mggysecl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2egztgbpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqhmmjck.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kmjjrxxr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jljebeeg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wciscxfh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewpldswg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2wvkaktmz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdvbqwys.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2weyifwlg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2uhjcmelo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugerviqv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pyhaxzar.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2whszztyd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmqewfqk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ytcoxsxd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2yplvovhl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bulzldub.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xozqoblq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pziheawy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzumkovt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ygrhiebh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pzfujkph.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2urkemmhy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uoaiepzt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2tliejcuy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xyujpkcv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2abtptujl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bdnzpcqw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mysejekk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wtvptwkz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wulqqjdn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sratgxrp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysqfemym.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxndcjyq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2admzqfgm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dxnapiqh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hyxnrrho.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lkltgwqq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hmazdxrr.html


<!-- 参考信息 -->