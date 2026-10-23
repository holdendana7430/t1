代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jdulmrtn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bgefkiiz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gytvdtsf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xwnegfmo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rnpgkavv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xgfncaco.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cxbcaeyi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jnubhbby.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hzrhsezn.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3phbkecur.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wjyvqery.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fogrhxlb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ykoulutn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rhrxwhmw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3vplytsiz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xdlsuoac.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ysngjott.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xevhesge.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mbdlcpbe.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wonkjpfm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wxvkpson.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jmseqgkv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sqygsfoa.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3swfstsci.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3yltgusyc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxshrdxg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ccmwspqd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xjwgeizg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3urusncvj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3bodafeii.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3rurcyitn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zrwocoze.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hrrsfqaf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3idvrqzci.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pattmvtu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xztkwuqo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lyxgrglt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yactbjyh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qeaqaqgy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mmguqxkf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qbladwmm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gmgbrngs.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uimxlxcz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xajzrqjj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yhmvnzce.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vssltyrx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ftatmlem.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3eflpkfoj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tjqvokot.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ablmznyr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rdpbuoko.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yfdddmvd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fztnxjgr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ggwbmgla.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3woyvjytg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dutmvppc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tuezsaed.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jbnuedqt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xcqaiwnn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cffegkej.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3kiiteord.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlktlkvt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oixuclyk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dluubotl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vfbodshl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hitjbszt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3tundngio.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bpddsvgz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3apbcsffj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xhfnoxee.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zqgcsjgb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3yrhugevb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3zqgpghpk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hhrpenjx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xwkthqlp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3farawpxy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tsqlxklh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3socyufrm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxkizoqc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3iuiorcaz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rjfvvviw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oyvnksio.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gcxpwlvr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3aefxcrgd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbuaddoq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3inmqubxo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cnfijjtd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3hvcyibqy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3tfskptwh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kacyukfv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ogkcntmf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gbdvkmem.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3azmsabsv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3egzbmnfw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3fkolbirk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3salfsxzy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xuhdzjbs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ltlvnjde.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jplzmubx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcitizhd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3fgljrqvf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3aumwtsbm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qdrlcgug.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3urkckbnh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3oevfmhau.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3sjhargyw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ylbdyzsh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gokbzdai.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rdytkfed.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3earlchmn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dhkoqbpw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwgomanu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lodjrehc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wetdmnnh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hpafkpcv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ckpftnqw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ghzmjzfz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3udqokqpw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tuclmkvl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nlabyywb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3viklaeev.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xihdjkcd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3govmydya.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bxbnjlcp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cpnvhjwx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dhmouapk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3calzltwd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzvtkcmn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3gathyord.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rjtafgrx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rswpmmrg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ggogsfnw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dnuosnwp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hylggigt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rguybewc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nowkunuw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mizlztyl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3npbobhmv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ebwxdpjl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wbmwqqma.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jllaxitk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ixzlfzld.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mnrlndff.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vxhoawwc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bmfqibxu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3sexxtqpo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3erqjclhx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xzjuwxje.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xieynnec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lldwrwzm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xxadpnyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyqupncs.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vnzcljxd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3unfnilgm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3atokxxab.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wyxqzken.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rdwikvea.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3oxtlowrl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wnpwvcew.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3afecztdo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3idtsyeeh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3urabmfbh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vhgvjflk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3iajfgtml.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3haakwlye.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evpkkzxj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3aexqzcta.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gzlthxmu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rpwstdwq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3nrziwvhg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fgwjfrkk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jzaaqcfr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3feqttgec.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3effnwmcf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xywebvnn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qcjsljfh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hygkkikg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3xxyhudtk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3olbxfonl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vvnpgmyb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kmqugtow.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3loudjcqf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lbdcrkys.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ycakqzmb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3qssebfdf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xnpazrue.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mummfjmm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ykwavqpl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iuejttbj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3cnogmpsr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uujgbxyk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xsqqoxek.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frqjhglv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xaltkigt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tbzcuckk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awzjvjqt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svudzfpe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqgryfff.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aaaqmebt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cbuyuncq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eoeirzda.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvghmgyg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lxrstsmf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjvmbtgm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3badgxusj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3txmfcryy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jksezigy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pdfynlzi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3onsftctb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ojdswcoj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hylykran.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3woopefkw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3urfmkevu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wpqxgeqp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3umupsnzn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xpmmgeam.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zhysbheg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3yygoquvr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3inzzqmoi.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pkzfxnft.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3shqezuvl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cwgmdyvl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qigcqrkj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zztzxvvb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fnntidqj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwtaujct.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jvqnmhna.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ojgckebu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cazjfyay.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ynbyplhd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rebenuhe.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewtykzra.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ryysyfol.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gnorlyul.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcmckldl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3euabdgkb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcgfbqpw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxklkqri.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ifhuwncm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwhoxavw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouiifpqd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gnnqmyqf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3veefamcr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtfjljnx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3drspcyla.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tkjelcgp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kucweoxk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xciawopa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3aajfivhu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpxioaca.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ahoxqewl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3dakhhefw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3zahznlrf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3gifnujxx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3brstcopa.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3agqqbybo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ostkvkiw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3veetconh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nofzelkf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ddqtkjvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcmttumw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hqppnzig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhytggds.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qqfhxive.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rrslbbmm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hfiqmvvu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iftvlbvf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nftviboi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqjmnlzp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3kduwripu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wukrjlmy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfdxbwkb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rzcjvmvs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wgqwlssa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylajuxxg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxdidaeq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pifxhrrm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3immividj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3adwgxacm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kxrczril.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kusnvvsw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3dljlfhua.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zwnpbmiu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3objgkzjl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hybtkyag.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3blmeifjy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3dzgpjbso.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jtlktbwb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pxovztdv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cwxqzmao.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3yiilksmv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ampwxrnn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jdzidbhr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3equbxsft.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tnkgqley.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icsbalza.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oecskgpw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jxjghpww.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yplvuzbv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nuqkkuyl.html


<!-- 参考信息 -->