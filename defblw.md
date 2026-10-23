代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rvrrwzra.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3bgisoazn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3adtcoirv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pqjnzuvq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hodvsdvy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3scklrrlb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jxwfylct.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ddvcnocq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xqcumrsm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xpzvhhgd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3siczofgo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3crnrpmnh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rkyaibxm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gbnbuksk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ayrdjsra.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tlpuotzd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gyrxtwdw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zbxzfgav.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3zslrcjfb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ifyjuvph.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kpicizix.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mholkwok.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gddzvtvd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gqebfijs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ptpmqsck.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3chmvkaxg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3negfcvet.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tkcbkuty.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ltejjpne.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zgbgnlab.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dlshhxfl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eindzpxm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hayliguv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ratahwjq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqbgrfsb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqxilxqu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hzakxycz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nerektok.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3bissqwgj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zhdbnurb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ljnbifny.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cxemjalc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3oahnrydo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3befsimlk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twevkiad.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aonftydn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3bfwhatxj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wkbxtwex.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vjscbmbq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3zozybczj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3kjitwsbe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rjkiuode.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fvvaione.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3csqbulqc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3aapuumqp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3syhemfin.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3cjiqbxbb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxfzippd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vppuboch.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lfadqadf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3eneqoctr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uqopqquc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mngqrxqm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ejdmqkia.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nmnxtikm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rwlsuvts.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3eembzwyb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kdmnqkgh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zwisddcj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qsrsejwe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3anhmaxap.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnvmcftj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hftysmki.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fzyjxjhr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ztrusoki.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ucamtqny.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3orqayedb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yhwbarme.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3shtifowx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnxcgdw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bdtxdefi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wigjcyrh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fgdfvsyn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tngklsnr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtqbijed.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ewuaqfwt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3qztrcpyo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lctdpxmj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3cdsvsqgy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zywcudtc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cjywlrud.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vcragmtg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yghuexjn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wlqjfilg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mxixnkdf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3aiopakju.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3pciedmbf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bjfisjrn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qkdtsfwo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3kyeuzhht.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xaxknatn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xhvxfutr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gqdamsfp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3boqlxrgd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vqdtxjxn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rjsznqie.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xrbnryyi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tcpluquk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rdvdvyel.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fnoouzat.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3onrsuixf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lkphaxiq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xuywpncp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbgvpwnj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rqqnhale.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tfbbephd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jhzhmefk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pxmnalns.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3spztqlei.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fpewtsrg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3awnlvmhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyclxxck.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ukqucxxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndgqkncp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lefqxqpx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ooxqjhae.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eshmcbfn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zedogzge.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fzxtqvtj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3snlsizng.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3acdgurxm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbkngdut.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iilonmsy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wnxrsfzc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3srbprdeq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3epbddetm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3iysqipkh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufxwrjqr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tmdwmuzt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3yckkjska.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3cadrnshk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lcdypsvz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3dsageeyi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xnxcpcwl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qfoeqzqe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3djojebty.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oqlxnsen.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jrdeixcp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cqgbzasl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fonvjzql.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rgangyvw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kdlvjsdg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jqjckwjd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gmrnrmop.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ztqenasq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xzbpwclw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mtaaxumj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qqrevgax.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3mnpgjjiu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nraxtzms.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ndpkduhw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rxvnvxnm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zeqfgdzi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uuvxiloa.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mifkulca.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ulfclpnk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ywhpwkny.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehznfeak.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wumxkcek.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrhgacgy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xxdddsmq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3waozhaxp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fpkhowyi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3osnmkqkp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xtqyudse.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewcowgsr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xipcfvrq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oamopodg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xffzarej.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wcmqjsqi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3hdioehap.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fonmgnkd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vxawxuek.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ecpqnhtt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3iyealneg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3hsfatihw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3thrsmcpw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3uegwurpz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dhelhivb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipombzts.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dfomkwno.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bazvtvfm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iuihecwl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pmxmzdmn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qvjplkci.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3umgobybw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dbuvlnnc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iurvmnpj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mcxbghbm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zkmoaquo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xfidbzmq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rzqbabtg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pizooxou.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhlhpinx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ovrtdloa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3cibxymvy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxernqep.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xduydgzb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftyztdeq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbgtukkm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gkdgnnua.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3voizbzgi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gvjnidlg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvtmobvx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qmesryby.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3utwcxcrp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3uqckcyad.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqbibzmz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yywuhhec.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zdwfrupm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3faccwvye.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfcezvwm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ibyuredf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zdydhhdx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ocsngfmw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lradvkiz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3gdfqxyxs.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3iwvbfqvx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zqojvaid.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3txnbbqfa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vwgygsxf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rfrpzefs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uihvyvae.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qgtgqamf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqcpcabh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qxemymxp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3pisqqffn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cfnlyqfn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gekzhiey.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwzsbycx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3prtkpidy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3evtnkpxx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3crfziyov.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jrytvvgi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3suyhddys.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3foyvrbzu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3sgthjzmk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jteybznl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3yecycofi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uwrwznuf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhgjuav.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hedtyxvg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3muxoszsy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jnhfrkef.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dlzoxojf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jpgfuvlc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eizyutdy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hdjyihbk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3syapgpak.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jgvdanbw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fujtnepo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mpyjlozk.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bhaggmhc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mlotwqsu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrttzvap.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yzzxvbzh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bzqeyuig.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xrgrrmro.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wzzlbteh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3juaceldg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3diakmpsl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kejgrvko.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3eaoblhla.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnaxldrf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dbpfjkqn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3clvafvre.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sofrbfks.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3hpjawust.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jrwxvhwq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3yjufxcig.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jaskntqi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dtvwqjza.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxxipxdk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jzdoubmc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3claoiibn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xbjnyrie.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3mjfvhypc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qmwqtwqr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tngsaszr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xwgobniu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3jxvtqdnc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3vmqccnzt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tinaxoah.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3izotkmen.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dpjifsiv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jcyxkmwd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tqgpjboq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gkbwrill.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ixmqanlc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3uxefbscw.html


<!-- 参考信息 -->