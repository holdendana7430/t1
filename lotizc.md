代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fdbkhrto.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3igtqvjry.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3nmlenqgh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3tiyatvzu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3yqzqvqjw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3llcrgffb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3mfrucjos.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3upawzivs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3prvxjren.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oznqvcwg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ondmrejt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mgxxpzvu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3uwgjvzth.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yftiahxo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mobqcjxb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vdvqsrpk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ekemsluj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vgeipuay.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dwwzmbpb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3btuhfvxc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3okwesuua.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kysqcuiw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wgjishrs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3axvgozyl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3novxuqsu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qqjzvfnu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zwabvmdz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3evtjjmnn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kalxqykp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tydznbyh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kxydyoah.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3slfkwtsa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zygtjrev.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fzwnbded.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hixacnja.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hdmvzmkl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3djzydzkv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wczggldt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bdufsmke.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3znvaqafk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3impymuke.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ebnpioui.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ahcdtves.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mjzowwre.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3feirnjkn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hyfsucnd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cccnmrhv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3oujhppph.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3eiwuosvp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jildwhyd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3oguflwwm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cwgbedph.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3nscykgbv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnpcynpu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bghtdrdh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oyfoewrh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjopvebc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ylcnlrcx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3iyyqclor.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uupnhboe.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jxihpnxc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wfdxqjrr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3tcbvulco.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gwmypxxe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jwpiqbhi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cypsjglc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mxwknapv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xsnbtoxy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ztncdfag.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3uxvldvur.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evvzybyd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3cqaawicc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gparmcrc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xbungarj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3trycwkrk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ukrvcuin.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3uhnnqgfh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ezxivczz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dcegblcs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3oimpyema.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jgtbrbjn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3caevztlq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vmfgrobc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nkynelsr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3zjpcpgga.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dwjulctc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mdxovjmc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mkjlgttb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3llwaiply.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3mdaceeki.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gklbskqr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3srevjaoj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3saynuwnk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3emnnhogu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hysvjvkt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dbnhflcp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qcmxibve.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pfekuwvu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zknntwsx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dodzvfff.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zbeofegm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wjafstth.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vykrbacn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wzvfemdv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fmzjhbhs.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3rbkxvhwu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3myudmyko.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ofkymbfk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfqepbk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3safodfje.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3eohbggub.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3iiflcuec.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zxhjttge.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3prxwwdej.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3zvqwjnpb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mzuiseiz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ongmquho.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bvdhbmye.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuqmrtnm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glulawgd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3toughxtz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ikuwtxfa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gdnlcrig.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cmwuzjkf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3muxxazwv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jgayabxd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bavyzden.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vpsefonl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ksqhknnn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3djkpdwcp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oqvqpgwx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3amsimwzo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bnyyqjuw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3dylhtjqj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fphlelet.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3haikdexv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aiaynpad.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bhafwtkj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3znghwujl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zpmedsqx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3upkecjnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvylrbxw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3tkunjdzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwchdsls.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3guxvroay.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3usxhvruf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wrerewae.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3aidfmkrk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qdjnukse.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vguayouy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gridoysh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvyaranv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pbwepkzi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3uwwtxkai.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hbneachr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rzsrauzs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwxosjth.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hfofmczd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lptxcecj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3yczilnbp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3cynezlfq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3haabxkyq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3aqmvtroz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zfamvptr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wgdhhsrs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kbashfjj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lhasekic.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rvsyrcfu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3pqiipnpj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qdjemjxa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uqxfyebp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xdefsisg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3oeqmjwuk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3jwvjioev.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kocmlwce.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tpxujcva.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vhetmure.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cbgfjueo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zwznjxkc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zvjphskf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3sxkaglgf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ezfgnxln.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tccrlsts.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nweqshfq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yfzycecs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pfrxdezp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3noczgden.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jxyoxvao.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwkogmqk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qkwelhvn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umezielh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vxdrbgfy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3knndpcop.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zmxjifbv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ekqjyvaa.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgoitqba.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlpegewn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uzbnebqz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zweeqdhw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ywrqxvup.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wnlcsayu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ziizcwka.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fqqvpsbv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3nqmndytm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3phldypsm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3hmduhdnu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3newasajc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lbrcbnsx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3asznujcj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3drbchdns.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fqutfcts.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kgqsnvyi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nwgtwlnz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fpqlbiex.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gbujyrzo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ncivyfcq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3clvshobu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcdfydbe.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kwpvpkqf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wsuzcmpg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zajkhcxr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zneelpyg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3uvmqudsg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3heszfmdc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3vbfoyhql.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zqmncdnt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3azrdnjrq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3olnjfzsc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqxxosto.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmifibzo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3lnoqixzg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jcwdnage.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwxscdrf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvsxfcot.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wnizitkv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nlnjlbgp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3agcpprsx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwcwyezz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjwduyxn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ydxtayfa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hyponfbl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvtaglnt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uysoldeh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vfdwyjhh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dcwxrkca.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ussdfgvg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3efmddxme.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3cbhfyqxq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zfhwcimx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xajwfvhn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ctratnlv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3uqmospwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrlttzka.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hklxzink.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxiqkbbg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ezreheqv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3zhjrbxcs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuxvcrwj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qktpnraf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tbtzozba.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3buzkdcoo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vpjuxgij.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tdmrckbo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzgfcijk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmkyopjl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qhvhyhku.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3czupvxgl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xywqltnn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ioxfodrd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wagmbhmq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kdxwqjpm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gnjcblro.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mqsaoypg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3yivubtqc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ppkpklia.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xocxtrrq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xfgbcfyp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3iaesbmwx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ruatdrjn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3chpkaelw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jyzkfpsk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uuittgcm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3krhmskmb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3aqnefkyg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehbltukx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zidodjof.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqhkvsbm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnfzeahz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hewkodfz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ycctheje.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sxmasnqq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3nlghvurq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mffomrnp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hyoscyhb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fpyhngtn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yahyrtaf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tosxgphc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tcjpdpwy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjlpmcfj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3kaqwuynu.html


<!-- 参考信息 -->