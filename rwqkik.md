代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cguysvty.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jervqayk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2excmmnms.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sxdczawk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qmrltrcy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2dhrgcpbq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lfdvezok.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pzjqlvmg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pvxvtsmk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kcuubtiw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2smjubukr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pwauhwzv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kyrkhawx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pgibpzva.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2udfmvlap.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cbhzmvwl.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jguvbqwt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eqjwccen.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2vxeyijgx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hasaaqlp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fnsrzwhg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2outwvgpt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rkpyuaxy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrrtasbf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2svrgnrbq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2hvfcybag.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2uuaesqar.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ktgqnvak.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2sifocuht.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mvoaklen.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ixndcszl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wcqpbzsm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2uzgxwems.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2trgwirvr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2elwludiq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vtovcnez.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zgxxmgzo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zqhmlyjb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xajqtqdv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dpzbkjhn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2lppqwndc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dyhowcam.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2kcsatmns.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bzsdwzav.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wlwurhvm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2svhzbuti.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2iumikkam.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xrzttaey.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2swokgspa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2foqeympb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2alrriiee.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xihkzphu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rtcsgnhh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hxlibvat.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dpejiiqc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2epamsjtj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zqzxpmvy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yqnbpudp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ujblwfuq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lliwjgdd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nqvbpmjd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2axluiive.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ilsknraw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rzhcyqdl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2wcaauiuw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxpfqjhu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fnnwrerz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wionszha.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qskquyua.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xcwnskjh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2iotbhium.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ttcrckhi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2utfbuhrl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioxjqjft.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vofdhweh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rcfiesvs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xqqwwerf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2iufjmpqt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2bzrvpaay.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccmadvff.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xpnycyyh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2wifcryoc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2muxqtcvl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2fuekfnnx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2utrtrqof.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qhadfnlh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2yxrevltu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qzrvsyit.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vakitick.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ylalakoz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2whpuwunn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vhzqtkmu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2taxwpyiv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tgxgobna.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2pcqsmqtp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2prpwrlty.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ombstlfn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqrttorx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2swrzxlbj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2uncftoyx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2eavsngul.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ijwblymq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yzuphnvu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2apftwnlb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lduruhzt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rotvjjez.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fadddxlw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rdfjwyev.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nuruteda.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2vjpypeoy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jepdcquh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jznytvse.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmaclosn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mmubbpus.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pjrzdbyl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gheyiegq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2tapxpjjq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bamnoime.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lyuegyyd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dvorpxpp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vjfpcylr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wuvgkkgi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zcfyjgqc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wxlpxpgy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tpqyswbr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bzjqesfj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wyzughuo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzmghxhf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ebdwgvtk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bbboqwks.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2gkwktajw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ybmtkjrg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2mhqgehve.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2bpmdkvwp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qsqmkirm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bkksfpwg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ltpyeqpr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjoijujc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2yjkufwnj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vbzbpcxg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbrlycpv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wwbxgzqt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ylwmgwny.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dnvyvxqm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xhlkojqe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ytsmenwt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2latdhhrb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vsccwyej.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nksgujae.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2taosjsjp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qwrlwoes.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vnugmitb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zdnhtpvq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wotxkany.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sfpvqbti.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ssyahimc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xajusqvo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gabriiyh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2czxpfurb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2keshftls.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2enwmbbte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agadlned.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2tihpgtsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhppsyqy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2trrdoqah.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nkjzmyqt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uliyngqt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2glwkjjol.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jzqxgqdm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bzuluthy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gdenojak.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbujuflb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2keebypwf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2swdfopos.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zpnoorud.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxjqdjte.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gixdwksb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysqasrsn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qowzsyzy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zukpgiyq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jlfqgiyl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2yupruiyx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2akzzuqmr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2huahgecj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ocaappwt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2brdhoayn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ylsmramy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lajzhdjb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tkxcoqhm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2muwioblq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hesxhdqe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2piljqzms.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rbxxmtyu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2pxxtenry.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rbnauobl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aglksceg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2almukkcv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2brylcnso.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nxejluyy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ohdqezas.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ilqztjag.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dpyprdwu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2edafemtv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmdamchi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evlptulw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hwheywss.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2nvsnpxcq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klsohwue.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnlbivac.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2utbwmhvx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fbespdid.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vrywsjva.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwucblup.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vadlbksk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mhtcbhoj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uogpyami.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mizmqvdy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iqvwbufs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2urtubncl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ghwozqaa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iiuxngih.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cokkjzbr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2exbmkawn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2dcghqmbl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nzfefirl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2eokglfqy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qevrrcjb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2rbmaoeyb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lybcnaex.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2elhggayl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qecwrlhe.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ubmzenup.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2eeiygqor.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ldrgodhn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zrpixiln.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2kkwxvbpu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2cjfrissx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkovtegx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qbxbhlvu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bvzamrpq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nblinakh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2guepeuct.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rxrirwdl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhpoxawy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ufmldrbm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rqkqqnmf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uelmdzge.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ewfktexr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjevkabj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwkqupin.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2biommjdx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgjgoppc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qudrvjqk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2icuvlxcb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vpdnitww.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dwrozsko.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nhbnpumd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxkvmexy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xuzktgog.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rwuamhxk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xejiktue.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aoicixcl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2caoybotd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2uicdamsq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2oidmaiog.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qbzxlhea.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2rgmbdeih.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xnrjypyu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qxdwtjdc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uzvbugge.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2phtaqsqt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2wrcjxvdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yeucjrcv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2vggrknju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qovzeniu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zhiecatu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2bkmjghvh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2hizuencv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdqgaxuk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxxjnlww.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ueweeehg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wjmjdpyt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2iaafkvdb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2henruccg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kltgtpqi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2frfhycev.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jywnuksy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnoqcmkj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzpstviv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivkaapix.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wzdxrimg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uinxajzw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pxxqghqh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2aprjkzdm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pagjgzxh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2egxjbqof.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2axlcrhgs.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2idtgiltm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2idoxcnjy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gtxjtril.html


<!-- 参考信息 -->