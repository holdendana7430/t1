代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2lvmrmxdp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qbggpwlf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nafskrvn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yyjlnutk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2oxwqxcow.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qttelqss.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ojennxqy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wsmjersw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wnouzlvw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nowqiwcj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ewrffbxv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xufzgotb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvcximjl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2oqcsjqgr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qiimembg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uqdaqszv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2uygxdyim.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2frhbscun.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ppmpnlot.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xijlktmw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jjhstjhb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cfitftmo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2uhngdijv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2odtdzozg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zhmrukjp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lkhxqehn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ylutxokh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kyppkhmf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qhrbiqwg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2pezksubn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vaxqdljy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dwtsfvmu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fruzzlsj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yuvonipr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wgbrbwob.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yfbbyawe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tnijrjui.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2upzvznuc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rjdecirj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vfjjjdvh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ctgqwlss.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2alwlhcwc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iixpglwg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jacdlsjf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2borbjbne.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ovvyuwhb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2zwzntxmq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2akxotbut.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xhcmrrxm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxjjyhaf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2etnevyuv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2azlrdkla.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2urwgwfvd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dpoojtfl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mttwoaua.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sqdxhmdn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jirvumrf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2rwsngacf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hlvjjpag.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2oogkcftt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2layfrkup.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2slqzojgc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nqttaour.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wcspgoox.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zxbehoiq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ildwencn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2cnjwaali.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ghxqxniv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbuutwwj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2giubnzhk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2fckktpgo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ibnklxzo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2zzcgmzlj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mazksuyb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uvhhosok.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2scdjgvwp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nfqmcufw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ffdnfviw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ffpzumwb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2doemeciw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2dxmslpva.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2unmfuadc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2rrqcpbvt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2iyiordeg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2diaiuqdl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aaovtpzi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gqabtvce.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2erjyijkr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2veyfhvfh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fvfvygmq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dgpcjdvy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lmbfcwlx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dakwktdi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jtguggmd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tfoonhkg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2npxmvbms.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ffzwyufk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nejxtmwq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wtsorpwg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bszoqrmd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2pzddetto.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dswqssps.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2gbjqklqf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yhyxggnv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cdzbztlt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yqfgsejq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rtonclaq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2sixufpec.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2klwsswjj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jobotvzl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2pqthkbbw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ejbovkfp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2touagifu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hdjwmrhq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kpmlxawf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tquztaak.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ettnnldb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jhkhytuf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdrjyjjn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2xzkocgau.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bcyrtaqr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fcrpshgd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mdnylqgt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2odcdbzpl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ewwgigjq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ltczzlbl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qyzcmeog.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zsdzhafo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zqndtypo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2hgkpyveg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2reifhuij.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ulwnqewl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2davmklye.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zbaxphvk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qznryjyr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lqgbgsat.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ltcglxne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvlzxuzd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ygjyolnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cojwtscy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qakrtaba.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vqakplig.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2moztfmtv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rzuiyolq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hwsgbexj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ybfnebfu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nssvsjma.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wigzwblt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wxzowvfh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fyxarqwf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ecdqzsnz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2okjosbvn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2trdhuuyd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yqgixqyj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ocgrmatw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2syrnmrqx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gqcusvwf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dcmjxvzd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2utadlqir.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rzwhhyus.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dzwenbve.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oairnpdi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fmwlbzmp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2duptqxgo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kiwlctkf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xvzndnga.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gpvzyklg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ykrudjov.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2omjrvrtk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2plzliqgr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qekqfkrj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rcudriyk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rvcdpgso.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mxwfojqx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2szppnpqw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2einuhtxz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2vprkosgg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cvwkikvz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pykoimtg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2npssjuoc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlvwspjy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zfwbffua.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kqjtlxkq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yzxwkrpe.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yziiefpk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zoennyxe.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2igtwjfgt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aetnomye.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyqclqle.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uxrjlwub.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hcsuazkn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zajnzubr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vpapshgj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xvkiaims.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2klafxwyn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fnmsxtbr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vhckicey.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2slzdzueh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kdymwiwu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2lsvyfzsq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rxngqzxe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2oqkkixhz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xbsjttqz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ytrzaoik.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2jqtyqznu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kjplxvur.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kmuqpvpu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wduvjttd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fcotgwgv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2tznmpvxh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bgsawrba.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vmdirupx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qanqlnmk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xjnoudvn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gbflncax.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jdvttmjq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sowrdxgz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ixrmrxkq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nouxznpd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2takwdvup.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tilxygva.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2neftimen.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqpzuvnb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ormwqhdu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tdrsfrve.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qynboepb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qfcxxseb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tctmfsda.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zfuujibb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryifpbif.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2izzljdjf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pahqzdly.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ydrisvwn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzeensju.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzjdiiry.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cfeblemd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wtdbrwxx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljjottcq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tnbggwsw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2brqmkaag.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tryqqhjn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tvustjpk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ctfnlnfd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2upmnwvan.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2affedtsc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uouwrcnw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2nogtbyod.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ulvmkmcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlhikucf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wtijqujj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekdlfwcj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ewnmvcdq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2evxvmrbn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfsyelxn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uyfhgpvt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2urfhgitv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tftqhnyp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2vjyuqfvk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jjgwritf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2giugnyrs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggnikvhv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2lekvawkh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2eswlavzs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fhfgnuth.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2drfngvpx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2osgxiqhj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nahnwjuo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2llirgzzy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ofiwhnnx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gfcaawkm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gipchryp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2huzdrywt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ibqgycqx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bktlavrm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2seumqkdl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zbufglxc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2illvwwra.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2unspudmj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ijhsytpw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2avlbluwm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dntmzatq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kocquvhj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghpfnkdh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dplqfavk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xwikapxg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2iefdwnpg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2icxrmaud.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2dicyxmdd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ltskqlwb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxvaxevj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pamvrtcm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnxshnzu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hheaamzk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2eiidqpeq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zqnryide.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2tgsrgofu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2iidldpri.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2bgpbbnbh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lqkfaxfd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ycxtibtj.html


<!-- 参考信息 -->