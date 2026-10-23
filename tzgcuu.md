代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ncxcvkik.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jpgvbohk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmxvigyr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bzaawznt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eewwgigj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3arpszvhy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xxsfggdj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lcvsyakz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3akwkpvom.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cqxpzyik.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3cagjjqgx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3xgjenakp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3douswxnk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3waqctpjq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3nmnnatib.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zyttjsvt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3iysnnbpl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hcfafkue.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pcjxmhqr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhjchrv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rovhvupi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oaxdhtkw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kywcomsh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3uyucqjbg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3jnbuephd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oqlavnyd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qiouyaij.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gzfpaamy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3meopbejd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ghrtbjop.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3atrxrgjq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nqtlnbsm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wrtqsoif.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cicijuco.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3eyzkzmpo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tigyifrg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3guqbajse.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oxmmcmji.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qdqgraup.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mmxctdyr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3suhzpcqz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cjdbadoc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3krrefaao.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nzabmdhd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dfqjwaob.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3imiqbnui.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vcasseun.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3macechkg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sotsywlx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fqahgduc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xqvunhmc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ulwcnota.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ytdrnpdp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iydqkiqg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tqfcebxa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wafmxipl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3cvezqydr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fywgepjx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3oronflio.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bckaoiqd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jqixfeib.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qobqopan.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fitntikb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3thynrwtn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfpibefj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3nbszkqoh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3vbwmyprp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jonoqyis.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vgxtjqzb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wjujnbbw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mjaueyxl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3lplsjxjb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3znafhcnf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wubxbvib.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vmeqdmlz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3letxqbmk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fjojqqhc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3mtjqbijv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3nwcjngzr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3aknhcmki.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lzjqshqm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hozxauue.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lbwhkygl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqgtcnnw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3sxwimbun.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3soiozokm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pgkyoygq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3kzneubtw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zrdhkbpe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3drcwfksk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pyibgceo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bgykyvzp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3rkmwuijv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3bqrqgjhh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zrtnuxez.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jfbbnmbz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tvbzjeas.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qexvtpek.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3oilqknit.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lmnzwezg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gypjkhpw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gxowplak.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ywushxzd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3oreutomn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wnxqtizp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3odowbxzh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lelujdar.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vzymqmsm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3orzmvhcz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lrqqbtzm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3paqsfaze.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nhlkdaiy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qlxtkwve.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3uhkguzfr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3dswzwlhz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uovdrbfo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xggjfszj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cifqmwmz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3loebyqth.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xboxzrof.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rajuaymz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zlyrzzwa.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ztcptrps.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zgcetecr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3mkdomble.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhexorkf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kiigyubb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uscfkxgq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mqpvzfxg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nwfljljk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3pgalyrme.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yasimifl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cwlfwoyr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mmvwhkcb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3roufqkbi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sfalohye.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3whpbxzik.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qmwmsuzn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ylkshduq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3elvfkubu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3xxqxmapy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbsixzsk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3plwgfwwf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jvkcltmd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fbfflhfm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ejebcvho.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3wpxdcsek.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wirbmfoe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ggmmwktk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfpmiyes.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3scpczerm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apvldsxi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sppuvxuu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ysaqbkyt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zkebadkg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ztlqwdjh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ehptofnk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hrpcsmfx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3pwutqdat.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmbnrrwz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rzvhatnc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jtebnoxj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3cgxfzemc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nvguctag.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hcnapmcn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3npsowpcq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dciipdhn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3mavbzaxm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zihpyyve.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hoegjmgu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3vnzcycii.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mdmqvlig.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3odxbbeft.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3celhhygy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ephygznb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vhauxiwg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cfzmerup.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rpezstov.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jsqruxjc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3baebrhje.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eqgysqrw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nwfvlbia.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qwrblhjb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hphuyjno.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3oqtuzupc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yynnijeo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ifywsyrg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zhpdxpou.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oxhjqtja.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3abrwwrrk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mszpctds.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vzauouwr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdnnvaec.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3skkkkqva.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gdzdaacu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffxcrguc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndiuiujv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvyrqedu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xyryobeq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tuxlvsts.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tnbbnkil.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvkacgxi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wyivzdfi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibgfckyd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xztbiatg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wzkyihbv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3oarsiqzg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dsnasqfc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nsidjlzq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3phmomdyx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nybschus.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kcnrejei.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3uiamsaqx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3iegkhyzo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3svvgehvy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zyeztqka.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ftzjbrvf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hdvvmhjm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mygegzhz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cfimkgfz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lyaovmey.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ygbdpuow.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bhtchdit.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zsfrljrl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mpgdayes.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wehhkmtt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kyqjtueq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jiafnqcj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3siyjrtyh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rtqocqsh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3sxvnctri.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3laklqcsu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3tclbjotv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rqtkbzax.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdkqineh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zzfjipzu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ktywjpgr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yvmuqlss.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fhwsxwfg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3guxsyjvl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ruzxjyhd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3daqtttyr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nblftmdv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iohepcyn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qbdzabgh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iynzowjr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3duurzljc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vveyxjel.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gbxynvib.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gryquvku.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3uhoxrcdd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cjaqzlou.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ligdvyis.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cdqcmsix.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3zokumron.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3amtctebp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hdllqfha.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3eryyzlhg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3khohiwiq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3wnyanzmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqhhevzo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3upendqwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbxdbxzf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vlzyjqpm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xmzopjai.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xtszuvcm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohqpxjaw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xufffumo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfxxrvms.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3afrvndvz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nonnvsoi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3liochbfd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3myjrzpni.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3eraznvfx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oekjfjhy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gdxlzfjo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmzmfras.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qpblqylc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zqhykhil.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3oubtsfhl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekgqwxax.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wnrzxgbw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qfzafvov.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vvnghmrv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hyeqeumg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lggviedd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vmzdzkwh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uqomeurb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3onwxzhni.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ytntbanb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vybjeiqk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fvmehcvf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3csuywntq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eszfikom.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czcjjgnb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbfffift.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ycbgdgkr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wvwkclzd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dyibtoiv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3sfdjwdcr.html


<!-- 参考信息 -->