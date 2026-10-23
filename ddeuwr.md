代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xkkfjnrs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3sfijesgi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3bcuxwsol.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3aiaafoow.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3uookxgmp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xcuunedr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3boiikggu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lwrlvpzh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3urkpwfee.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3smxtnrdk.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sjaxahws.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3skmuesha.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ygzmjryn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3olsakysh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ydnucitu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bnwhnhmz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3scgubqdt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3szbvhfhk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wbyfszye.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tqlglorm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3cqltghjn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uavobbfz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3zvfhwsft.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ikijcuvm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pmdgpmto.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mgwmfnwf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xaevipqc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3osnlqgqw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rrvcwkxe.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ujuhzkda.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3frhbprwg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hygytttc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zunnzouk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3emmbgzlx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ypzbepat.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bvwkqfbv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qsoezkkl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ioikvorq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dxcreilh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sjgafygd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gblxeyxs.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pvzmzzwc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pxupdukt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tdmsmuyw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3akxicabf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3easolqwi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3exiiozey.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kgisfxrm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3zupzngkc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gynksrfs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgcylfvn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3enhybndz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3euqluqme.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ghbmrduc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3owvkusey.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3afvqcyzb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vgoegciy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3yfbmcics.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3moignbui.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3razonmvr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3eaoxigqj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bdeufncj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3iiabzxkn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3blkshnie.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3obrbdyun.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mqacupdv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3crtxgeeo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3edxzhxpn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3grxmnhql.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dgblaqxw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3qdetwhhh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hjcojpsy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjrallc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zejmhout.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3razxazcy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rdswfzji.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vodnincm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xtaphtyw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3apvkyupr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3djpsscoi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cfmpomsh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cplrqccd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wpioquhi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ujjqiqik.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3thlvrfwl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pmevaagx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ejwfhmuo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cepkzrza.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3xjtcpydk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gooceoip.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jnmytcsn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3cqnoxyzv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nibauyip.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gyyllkhj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dmeuizzv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fxanvirv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3strbrkkg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gzesgkdf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dwiziddw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ykxqskje.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3nvvxszwf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3urjranwv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3nlgtmlqj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tklibwsj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mzsucsbe.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ajruyfiw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3mmdpksxy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kwlriijm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qqffvztc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hxhiiocv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gxpmnsvf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3cecnnneo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qmsthatk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uknczeyi.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lphfmenm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwjpvymt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ngxdqgjg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3krespqfl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zidqwavm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tzjyklqk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qqkzwahz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gkjmbgfo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hgeqxxmh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wpwclcdf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kgovorvt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gerajick.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rbxytiib.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iheqzdwk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wtlfmlru.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xpsttmew.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xdnajscz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tpanzydc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kziloqti.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uizzdegv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3clxkhchz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ttqvzgbv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mhfsrdul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jafusoap.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3rfcqlldf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3quzuqroz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3cnfravxb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ctcafiav.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xqhlxqeg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vtecomwe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ybgzzpvj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xskusdog.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xxpajmwd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ussyjrks.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lxtmkaus.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3eojiujlr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bmyjlzec.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqjhctie.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3aktxkmpz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcwijajb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cavdpnwh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dwacfdsf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3aewnyvsb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3nmpoanpg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3lgfiojux.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zepefkiu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uhbwwujp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3egdaduqt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bftxvcxx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gcndgnka.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3byhtmfap.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nbuclusn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dccgphpq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3avpwgpwd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sbmcyacu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3grmixwqm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vxroypox.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3epnfwpjv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3rcgmvnef.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3auuoyldz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yszpmoni.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3smdycrgc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3temukjdc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cachzztj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yabsopkr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ccsjrmvl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aclifkcj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wuhdvzon.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3yrqkzmla.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cuhqjhqk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukkklios.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqzihblv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oznbrvlm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sxgzovtz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wptxhhun.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzujcutt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zghkxrxf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtciehtw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bytixlua.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fgyxuiwq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mkqbuesf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fckcnwkv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ngbltxiz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ybzmdhgt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lnbwijwp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kxysfcvi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ltheptpi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fnmwqyff.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3yemegfdn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bkxjkwlq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ihvbxlbw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vitnvzkf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vkizrihj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yaytcdid.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jankwnst.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3feorwats.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wqpwocuu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tnrxjfqe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zqfdxkfe.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snbvhjir.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yefewkuo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jeeyrqnl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kmpnjtmg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rlvkusgc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3obztyvwp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3isuxtmbs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ytnxwymd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xsdahkwo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rewscyjn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3glizjfwa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zaeknlqu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3srldpchp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nxmeqrmp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwspqayq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mvkhkvcw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgibeqnp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3crzljjjn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxqocqqq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rfhlhanq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ccfzesaa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3owbylfba.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tffbunsd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3aurltnxm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ombtvbqc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wmhyoxap.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cqqprsvx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3llqvtjie.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tudvghdq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vffcxdbt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uigozsgd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vevethkm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xrzcuwwn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ehorqwku.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3gmgkihut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajzvixqr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3addzteoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjeglrfg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rnyzddjp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3gtdczfga.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3txkahkcs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jhfbtzef.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqwggfpb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3meomynny.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ksdmshun.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rotgancl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3asyfixks.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hmsktzsu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ybamltre.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gdimzizj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nhrbpxnu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qusejxpz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edwwcsjo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3skvlvxca.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tmavbrry.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhvolmrt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ctblayca.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rkiqrkqy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ushuwgfl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bckvkcjn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bcydpswn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jmwkvkcf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3phvdlewj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hrfqltnq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bewsmbgn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vnmmhcgx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vwaotoxx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fnyrzvpe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiiuatgg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxyzgxtm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bmjgludw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3smhpnxqm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wdtmdpkf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jzxktcll.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3tvddibec.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qwqcmcnc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lhuzngxa.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqqorgqa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xegbajbr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkhovgfb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3dgzbgngi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3szypiodt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvxjtmja.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xyczjaqx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3vwjbxkgd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ewdjgbbp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mjdhthvo.html


<!-- 参考信息 -->