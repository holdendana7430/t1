代发 wailian999

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3vmbsvgxh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ttfixutn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3nplgpcbq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ldkzihnc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nzvakbbz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ltegxgzo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hrzsgogp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ihexssgq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mmlzkdge.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ielstlxn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vlnsoxmd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3orrpvcpv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bkvpqrse.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nkkwjroa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3pfhmwmqx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxhravto.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rpyupgvv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3kalekgbo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fsvpqrld.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xpkrlduu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3wjipfcza.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vfxwgexa.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xcaqgjzf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pdxaxlru.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3tmmpanqf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fomerrhm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vpekvivj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fdaiowtb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywusjhtm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3uxlkaqsb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3srcylvze.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lajrlcuk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3upldshph.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3rhgvfhqn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sqqairaj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rgpnawyx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nhoslypd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3njwdpsdn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3htsegpkp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jyozlbhq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aipxlexw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lyknfobp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3whgpxoce.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bquaijez.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3oghkaxle.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lvsiaqis.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ecppiklc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3eqfmovyo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dqackdth.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oseqlrqr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3flkslwho.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nithuevi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hrrjlilv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3slbzpxzj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3oagoibwc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ksthqqqc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xwzwydvw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwkengko.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vhwzmqjh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3kvrlapwl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3krhbxazz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3msqxlhva.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3iufjmrgd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ekowqscy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xevrfvwm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnbkyhks.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ocwlhzgz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fycdigco.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkcjtlum.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mqdevolr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3aawdscmt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3btsskogt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3zermsmit.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wbrnrwll.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bxpojfyy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3lxqaytfx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3edwcxihl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3legcsgwo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3denufoit.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3agybwwlh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pwyaldwf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bxuwmppx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rcvzabfb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3kehyxwpm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jmifmhlq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3fniqyhpy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3tngexmoe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltorbfeb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jsybujuz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mieglcaa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hoybsekg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nqymtfqb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3scpsdtzi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wbdqgmoj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ywyraddu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3urrmqsqg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rcgfuuvd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3bbudnjmz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kpdrkyfk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3limtobzp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cocwpodp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mujhbahu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fqijktit.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hpuothqs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhxzcncy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3grfncmvx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3favxwhvk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3oxohwojs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ckwiepwd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jbpxsjkz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jzbxknla.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sggewrzg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hzjvweqf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zhllpmmp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3toytogna.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3diflufuo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nlvmafxx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3levwwujj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jzzwwqyr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wcrpszlf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zlttbkpn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ztnxqobp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3fxkjlpzi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zzmfjisy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qdnwukih.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jktqhmsq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mcitmevm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bdpffxad.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lxtqphmm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cduhcynp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gqquvlpa.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pffvtgxf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3azmydvgc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wpbozqnc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mmqmdncd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ddndalie.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3omoyflnf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bcbulgej.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xybakbyu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ypmslrqv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lehkwcig.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xjxngfra.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3prkuhqsl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jgqdhuij.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yxxcshzz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3uyhyxwnu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hyynwfit.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tcejkvbu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dfanhwjq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gchgrejf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zpqdpmrw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zjwdbqyq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pfwadaif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlqkjbkm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wfdpqabk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwutgdig.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qcdklmxb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bdzdxyxw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wfofrscr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3oygwepmh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yyaxnwao.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3oleatjai.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xavvmroh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqnflfxs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gdzuxnfc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3akbesxaz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rkbvhklf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eezfqjun.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xztttuyt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kqaugoev.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mtxnlfcp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3lipgludc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3yiaogqhd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tcaonvwu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zakpnsgo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3siqklhbo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lplvnbmc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cpnijlia.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3weobpppl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qcurzgwd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ooahvdrz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tfsobsrw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kpokqryp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bipbyhyg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3keyygxsv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ibynhpar.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fimrqarw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mxlmukwr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3logamzqj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ysvphwvr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3etfckaro.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3harvkmzw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nsxcyiih.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3erdbiaau.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fstyeszr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sfthazfk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flbavjmz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eaakdwbn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3raxygbgl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydxfnkuk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybokstgj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mfaowhaf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqaskeen.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3khheqcfb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbokyuuq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbmtvdlc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hjrroxlp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3crkjxrtl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qgpzapkv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sdmcfyws.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3yqwxfkgx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dnmrtkpl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vfgrsxhy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ngsonrfd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3oqeuuias.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jrofrhwa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vocddrty.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3llzsfsxt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ndhbvazx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3phplmjdh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ultozfea.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqhwhtim.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ubelrgea.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pfbdbuie.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnelrec.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gtxgwcst.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bcywtbcv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wdhagzng.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3yhqczckc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pujdvvlg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xfvlfthk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nvissuge.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jgrqodcs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3arcvywyt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3cdsyyujn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxlqhymw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3geooactc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rxggcius.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rpdwejhz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qpetojqv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdcfsozq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nuabwfha.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qbwmzmmv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vjnvtelf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhhtomgb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3phfjcmaa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3yammrdvj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojxlaxaw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uuinajhj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzaeskhq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snkixtij.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hecgogqt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ktoowwhk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjvhaknx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3cctydozf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xqiwgtax.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3efxrpcoa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vuxjujwg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3spxalcsr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3eaapmusw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3bjspvkaa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xybejxeo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jhrrunru.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jxlebdum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugbjvrje.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jtravszq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klkyleoq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lmglqqtf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3vjbbmdmf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ollcxrad.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3psgipmep.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3fohrxyqe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqsuxlmq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3olwdqkov.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hggzppjc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3krnrtilj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3jariczbq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bopidtda.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlxdbjig.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qezqupei.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qymujcjy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3elvoibml.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3blonnvur.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bbozkcnv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mpnkslul.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tsnbvvps.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gfefloxn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ejvaelah.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nvrqmxmk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lcmmuhwb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ghksznwr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3oixsikoq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qzaslswo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vjyafmgz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qxhwemec.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qcibjvkk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qocythea.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eewovwef.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obtzrdvr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuzpqpsc.html


<!-- 参考信息 -->