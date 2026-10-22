代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2waxanjlv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2cffjvrgq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ddhrcxfm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2spgvpoeb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2escxyarh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ysjtnwlu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mibrgwwd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nviwcwil.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lptycbvb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lnjedalk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ucoqlzpk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2krnrzkto.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2vqvzaxnd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gzznrykv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vgbocnzl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ciiqzdyz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jikyurlx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2nrevdnpw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rsqftbua.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mkkznohp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2psvagytk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rsliokon.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zdadlmli.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2byhljhry.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fwzolrhp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2segacmzy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2todomlhm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2esucgacy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2msrihwsw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fknmnttk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ztepxdpv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cudevuvp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2sqzyxroe.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2xcxqmlbu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bhwtolqw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hllualwu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qeueedtu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nprdrnud.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gdeiraaa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zbifezky.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ufsijcwq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2irykllci.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jaqzlhau.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ldxnpsae.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ufdveeja.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gnzonjpn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2palzaufr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2schikyqz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tubhiqjp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tknencqo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2iutvrlkj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2abpiyczd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ztoakxix.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ofnhupxr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wbpwihtl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhyodliu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqnolzzz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tbwdmvcl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2uqqiqonu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sosoukln.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2yzlwukzi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2dvgvasra.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2yrbeifbd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tounaisj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxugpvgj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ezwlrmxa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2sdwpukfk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2uhvjcuoa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gozqnmjb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xdszuthe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ewlynlyd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pejiojai.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yhfmxloi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bqtwpfph.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xglbvrnq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ybthhytr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2okcrzgqw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2yntjnqcn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vfacvbpf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rmrxvrtg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ahnroidm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2axawnugk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2erqsfktv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nekvfvxe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ricrxtfd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2vtkonqhq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2chkjqrna.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2tkyshkmx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2keojvovg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2baubzryv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmadeweg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qaeiqeug.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xticfwbv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xqbmktrj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2eaxfdyza.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tfwicxci.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ffetgxzd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2brztcxdq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2oexbdjdx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mexziham.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fhcqdktj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fzzpfojd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hyihnzaf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2heprmdqr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zikeodla.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2epwmqitn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hrhrgqlv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2antzymgt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bpsvbbwn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fpfldbeo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rytwhmww.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qyfbiivu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2dzqhardy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ltcscgoy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2rstkjuqm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hllvllsf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2izertccq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mptqguid.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmjchgrv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2menzdrvf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mlvkgppe.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qfivffyw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2rwbexpku.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2udqaqupv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dsifarpn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lmuyyljd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xtpzkvnm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dnndbhrm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2frbkatis.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2zvwtvfmk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zqhcdrsg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tvmuyuuq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jfvvgktb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ovukwmch.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tffeomkr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sohqukns.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qwfvdjyb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ssnfagmn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ixqbmrzv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hkvorrgp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ofszpcka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhtmwoqb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hfkfzfyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yuuqzlpn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqqjicar.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2lqpnflxz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vamptusu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2cijplqaf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2atyidcxm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xxzbbvyl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yjrucgxo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2omasenqr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ecaiwjal.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ssrxmyee.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vkmxcvjo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtqhwahd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqgkccnp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bscgafuw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gzpswotw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qkzjswvp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2guqgrpxc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fybglbad.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mtcztgjh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2fnvwgffj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2isufaxvl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2otykemhy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xdktmaoh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xgyhwryt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2drkuxsbw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hnuuvtxu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vcgveilf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lpdhpqlv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2emmosgjz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hswicqhh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sdmqxmsm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eizgauqj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2grwvihbx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hvdozmdd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zpdhzmjb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2iqowgtjj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2mrlqbbib.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2umflrxgw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2llwxwmbw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvtnjpff.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hxjcnabe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2etdzyjne.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2emkugaur.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pnalxbqb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stsswfek.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2nfuwzghm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2waiydaue.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ywljexdv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdyahnni.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thdtmyss.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ukfvuvzx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdwaizew.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tcdfyoop.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qkhjjewt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2yjmawxim.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mcrzkkto.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dovranvo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cpdngtec.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mqusdkts.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wvcwduiu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tktwplea.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ozqicnto.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jpttbxgt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2nvcgljkh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rqdovuzs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2owqrvfbo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ilucmdok.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xfvtmdqk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tnefnziu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bmppxeyu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qdhsxkem.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mypechts.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ghauzlpb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqeqpsst.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xyrtmubf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dlhuurrq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2oldxwkmc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rgmfiuey.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2osbrczec.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qrhntvaj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2vmzplcud.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2iufvnglp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwauhsde.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iwximror.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmwzmcsl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2enoczhar.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2tywzwsjb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whxcskag.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxvnvfpr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksxqgibt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ybftxdbu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gueknikx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mbqbbprq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lcffjevo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqrawnxy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fuemuhph.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jzijfymg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uympuyft.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rfgdhfly.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2drcyvbro.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2bfjntojq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jyqmcnmw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wbkffzvy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2apoxfhhc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cmqsvxiw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vxdcgefq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bsizvhhp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dvvabdvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlakhpqg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2couqdkqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eztdcmlz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mgecqdtp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2zusjoohp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjmcmgvw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2aretocyy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggdegtay.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltqskozo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2lnzdxocm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qkhkaesm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2asbpoxmh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wpzmqzwd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2sbiqikbp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vxczowei.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sciqrqzx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ouiesswr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2haowdrtu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jljxlcpc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yemwyqxk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obtcgygx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2rdstptvi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vvssyurc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2poicmklg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gkmsorhc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ewfwbafk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wgyhxbem.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qqtrrqac.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wblyahna.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ifjibxnk.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tjuqfcwd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hlhbhlmu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rvrmpflb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chsdveuy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xqzfcdsi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2psjyzeio.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wwlrbtdr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljeiwjxo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mxblifgj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vttrilea.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nsjyiwty.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zxsdesgz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oriwcexq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tqrxlfqt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtvezdnn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2riutgqqf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2syvtyttp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2pujewxab.html


<!-- 参考信息 -->