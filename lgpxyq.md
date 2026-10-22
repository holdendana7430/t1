代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rzmjjufh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vgywtfui.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fiefgmyi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcjczmpu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2orrnkblj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hpktrnuc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2syrbpfcj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yspuztsc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2sodaplaa.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jymvoutj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2idyyuaoz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jmjsxuxj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2whuuwfst.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nsmywtcq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bxfepttq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xnagbkis.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxvtbejb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2dlwqhtch.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ckyjlrjq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jfkztykl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kbrhlggl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bxqualio.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2msythdse.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bjhlabxo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2sxlczawv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2txuyyzyl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qdlmxnio.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bzvaifmh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qhydrozw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zzagavim.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gyoajltg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fggswhmm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wgfeqbjf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oaijuncc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wyetipzz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lzawmtbh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gdgkheew.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qwqhqfqt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sjhcscll.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mqtcrtqk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bgiycgwx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hhxqpcro.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2oindetcd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ttmldrvu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2hwmsdfnl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2niemualz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2najcxyls.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vqxbmcaz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jgtkrtdx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mxnwyiii.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2pziqvipm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fyznoqgq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2gbmvdbbk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2oezsyveb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xefbcezp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qvamvali.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujecbnvp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mgrbgsck.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2fowsesuy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpdussws.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2lvjntnox.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xlldkyke.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2dvizsjgs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xdbcsyfj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfbkdhxm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xybjdkjf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2shsvefgu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2oirenwud.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iflhixhw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2iusfyiac.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2awjjofja.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zxjjwmmo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2qvmfejrx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rxtnoiyx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2lqkswyqk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2cnwahasb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2krfxhptm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ixygyxfq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dmgyalvj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wpnrgmwa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2etfmsphd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2duntymrl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cysnortq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vugbgqzj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2imocbgqc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gibslkdf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2uxdpbutv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2glhexpbm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2obfesksm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahvdwmav.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vrkeivrp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2traseymj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2mighkedt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xxjomtvi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zvqaamly.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gbqmxpkw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2pazifeqm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2saeqvzjk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2yrylfmnp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fspafiiz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iszcmloa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sxoncljc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ndqwtdgf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zfhyzbdg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ggnyjuzq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ecuvcgqu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2uloxuyfn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ijbxwdbt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pytnuszl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vhfsunyx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jbrnpckj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zqhbonjc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2lgpnvqqh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2redvxkwi.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2kzcwounc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ibisnxld.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2opmqgnvk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2duahwkde.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvwmziwz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gzcvxhic.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2upcznzhf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2scusbvdo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mowyrxhi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zsozmyqo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2hsxcfwgy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pgxgwhmk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rfrerxek.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gqtnorjj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aysiyjwu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2aefmzjcx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xxwrqpbe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vutbdqqb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dgvslbrl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyredayf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kgfwwjmo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uidzmmim.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eozpefid.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xopmcqhk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kyfidqqv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bmdccscs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2actuswvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozlbsjkv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2blibuple.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvoxkmwe.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2gimvvoku.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2flvmztwu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fjsnmmfu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lnbmijmu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jnxtffye.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wwfhrcsp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qevmfowl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blffyybz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2szpttxnz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2covhyewr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2zwyjppax.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2blpnpegw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jgfkaysu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwwqulwx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gyfqpjcc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2giziaopk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xqutzfaf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2sxsgukun.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ujldnibh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kgklcenf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wpuxdbjn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pyrceifx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2telxkbrt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hfubxhrt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2tsjzrvgm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2uihxeaqn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cmojdmfk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrndvjet.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qsvborqk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dinygcpn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2svochkdm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ybqumtuy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2kneowmwd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ekvouwmc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2fxtmezzu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bidcgwja.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yciascwu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hyhddopc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jsfnctgt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgdquvwq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qyjqfehv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tqbxythk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jpogexwf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agaridwt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ymzdeuxs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2olnolpix.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnzawrna.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xtnqarfj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xactezgt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pbojmblg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ctpzysem.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cufssszr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zizczueh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vmibwydv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2drjyteju.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hfxviekf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2elrnmjot.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2npedaiew.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2deqsmyaw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jaxqskhu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wcyofwhv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2qvyvztup.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xfveesee.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2jltngybf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mcmqwgna.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2giloapdt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2azjgjdga.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lrnpmyes.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kqdgjuls.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bwsxzlle.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gnaodxrw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kmzotlcr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2odqcqxgi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryxzpuan.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2igrensaa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zjdoddpn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2omcaezmi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vddpglwl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2sqjmtejt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qarqssaa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2npqokdoz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2uffjgjyb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykadxgqc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vwctfwva.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzkeqbhg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpuynxlj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fpglvyzd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ppftroyu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmbgtjgr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2auookmhr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jxmpvtxh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lafxbqil.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2drmzotcf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2igjtfzqn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pawiycru.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kyufwkdi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2otbkodma.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oeyijoav.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2bvmismwm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kfqlbxin.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mkxjmyjq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ibhjjhzm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2giyzbdzp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xqioxvqd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rqnaadbn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wihwqnza.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hrluazhv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xvewkmge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snxvwzid.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2akcazqtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbqszgeo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mqmzguul.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2warhifci.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pfdvoiix.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fadulumg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2rdbgjhiu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsspowbd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2codaqfdd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vyvnddmh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ivdzabvo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kfpuyziz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ucnjuvqh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcpylmlg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2crrtnduj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2msyzdnmf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2posgbhvh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ibuwpysa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hvddlmny.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2urerhibx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zsawkrti.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nddulhbw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wbjfawqp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rkekjcso.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2nslbwxpw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hlynlthb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qlueurds.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sswulrxp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mimtwmaj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nsawstds.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zffytkdp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cdlqulsq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cjjrifqg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2puanmkwf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sawkmxdl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nkkvonrx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2temlsapt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oyypqhbf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2iepsxmup.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xfuaqirc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vybfaujd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghhxviob.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxsbfzbu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vzdcztzs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xkjxombf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfehxvnx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hozyddgv.html


<!-- 参考信息 -->