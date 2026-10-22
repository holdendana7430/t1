代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ejieuniu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2oexccvbo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2tungctlx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rjkcyiyf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2piqklojp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2taodvgvi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qumcafxv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ohuvtjvq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cvchmsdn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fonxrhrp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dklkacvc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dujixkfc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2edjltwdw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2uqaewzkj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yvacmlls.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zehelclw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hapbvfoi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xohdkxfx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gnvfaiwy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2phkdpejr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gizudwoh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tfbozkkj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2rhlaheth.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vppemrvw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mucqjkow.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2npccwohm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wtfdmpab.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qtzktrpb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2gaarwlsd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xdpzxadz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uruefwip.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tekvkdbc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vomvnihj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jognksxo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qvklbflx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jjuocfku.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gwthanmn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ijpuoerx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cawbvqef.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qafgfgdz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pjsekixv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxxiyqug.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjaawmzw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2lphwajyv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vdsivero.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zskibjir.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jbyznatu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ekvhueyh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2okppxvai.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2kraaviax.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fhkkumub.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zholdool.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ffvwkarx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fpxejugn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ttcejgzm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2akfmnfgm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bdhedqdg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2liasgzsi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zakylmdd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2kiyqasoj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xsamkskh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rsrdkidq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ttxdtqgr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2haaywmxy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bpulklot.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2sblfrppl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmgbbyky.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xfdwfevi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ibcffbhl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uopqgwdt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2disvacxu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mchdapri.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2htloauhf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2obgxhlqq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hhpmaahw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2doczqaor.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2sfcjujwc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rmwszkel.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zezvuvdj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jtnwdewh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2usfhjhfw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xlthtorn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vakehdbo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sroigtaj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xrbvhnff.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vuhwsmtu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xnezescb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xrdwpjht.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ntwptjsn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aznlvasz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2svmtlqio.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wwislcyj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mgjiuxml.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cxmoczvm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2sriefmhs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rgvsspfb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pzbzzqxn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hbtlzamt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jiomofvx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2xqedhoww.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xqfjqjdt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nvlxhaed.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pywchkkh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fexlkaga.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jfsxajib.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lgnenjny.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cestcoqu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oxtysxmh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2fmyeghvs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2oacpciht.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vfuarsex.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2uwsacind.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hellqjeo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdjiucbz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qryjcayw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wrpiwvty.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ohatqgax.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bzqqkbnd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2krdndfhh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2rxrxpouj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2jghycifm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aumyzyml.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vkvtkzwz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hajfghbv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vsrdstps.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bgulhetm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rczaiair.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vrtlrggv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ipqwmkmx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2skrmtoej.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2itqntdzw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2odrtrpzi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2piahgdxb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ndhisjhl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2lcbqztgg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2esrgervu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lbonhfek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsdhgvjv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tvurcmlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdnaiamb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2trafofsm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2eugvkzuo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xkildaxz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fwanfspt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jgckfhyo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vfrvmodw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2kfmazple.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxglgxvn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eolwngqk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2owcotfcq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2gsifkmee.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruvdxciv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbhwncmq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpllinjy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2labweihl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hfwdwqds.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2saepaxkt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzzkcbzh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mwrcbfau.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jtglpxtr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tsfzezzg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zongjzho.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nulclhvw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ahbojygp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vbghqobv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hcmwhyph.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2deoemsmb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2twcdbktn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qzkhvxwj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tujfzuor.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gnagvhsw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ttvdpudx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fhcaebop.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2povjvnnp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dnissifs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nnecskcd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ycpxnvxd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2utnrxgww.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2leebadhw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryvmgypp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2weddvkbh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qfckwvvj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2arnmwvle.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dovphcjo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbuwypzj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2nmpduqxi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lugvnmrk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jpiucxfb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2doaebdml.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2phvouubh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fuwsyvhq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jiwiuumt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fecittab.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2azodnwfn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hhxcrzcj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mjyecwdb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ujcgbvsa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mmcixzds.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xzjvqtnj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qtslnrjy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jqqqnhaz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2iolxtthj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2efslmlyq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2hffblebk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fwgmphkp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmjwwcwx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sxvwxmoc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wlmculwa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uvfbcwid.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2szttnuwo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2qxckqfiu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ndnmolzu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hqpcftof.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hyofsxnl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tgvfrudl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lypiciyu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2upqezmax.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nqvmeuvq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2txyxkwnq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dmdntrya.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dlmvxoeo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2sxuqzddc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owuzvjxd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aefexvpw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zwijouun.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cifrsbsf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2symgtuxw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2clixsdgg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzdengyp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2repbgvsu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tanyoznz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgbinzup.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nlqcjuzj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtbejppg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dewcwjcr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zrfmbfah.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tebtaazq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnnbbvys.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hnhrtfuh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xcznrwhy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2klsrkrka.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tjimnzhp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2argzywlq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xkpeihjq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qlwmtidr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gwbhwdmm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ssahpgfs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tcxqmajg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbixwxph.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2exebfnwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtckjrad.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lutdmovs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2zxafggbt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pqhgvpvx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qsjlskgu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hlxtwbqh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbterhhe.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ulymbdkg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2nxqgqfak.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggayxoyy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wavdgmut.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2viosamuz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hopkvrxt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldyontiu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fjcnmmso.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzayviro.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ipinfapt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wqjneymb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qmyxqzde.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wpaaawxr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mqchdrbi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tqqrkelc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zdvoclql.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jdyrrccd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2nfpdqacn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tvpxdcpl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2altjqmtq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mvoawoyj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2eypeqsdd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ixfmftvg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvkahrrw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2itfxbpwf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2upafvasg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfcmljil.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ytglgkob.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2guohxsgz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cpycwydl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2pffsrshi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dnsxhnym.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvthznny.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nevdwqjn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxybfzcc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzluawbq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kensjftj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2viworxjc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvjvbdvz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wvqzgxlf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2eldiqzpl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezmvtjgb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dvmsphpg.html


<!-- 参考信息 -->