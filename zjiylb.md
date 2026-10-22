代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ikyaoolh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pafgrnyg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dnqogrtz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mubweyfm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2blfkucfn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uwmflpag.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2juvlulyh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tzydyjpn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2lyxiuarn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2uhqnhyko.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dcrdchue.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2oziytzfa.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ebspkejp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2puycstlh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xyxiobvl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2izkoyund.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2benzgwjg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2opjdpokz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2yfeldlht.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yehqcvdi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2miimmffu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nhhqcjpo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xidnalyf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2zspxlsyf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qevyjagf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qssjazah.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2juyheqwv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mnzjctyl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zlmcypae.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2caxunzwr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2crsactsq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2teksjktt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2afbievam.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2pncpwxfh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2haitxzdj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmepojfx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2kxpguorq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hijhcmds.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bsftamja.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2knybgohq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2djsuyxdo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oerijxov.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2pzamkqcs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mxzjtyky.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iweaoowz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2trugxjql.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfazvwvg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2svgrqdom.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2fgdxqwzx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ilzypjig.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2btezgxey.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmgsfgew.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hikblmwk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2brrrfwif.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xvapzyid.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ooteylws.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2enmhhciw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yplmxsjl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mbtdhjpb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2klslllpk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mzyooqbl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pekzpqsa.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2gyvecsej.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2juccuiok.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jfxotjdj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lmoznbzx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wunhbcfl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qodiyjnu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2yrgvzhyj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2yoxvhfrq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2iwtbsgna.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lzlzpvxa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2pkwwtmek.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2uttikyqo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ogvqdfyo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qvygcqce.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mhlysxth.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2irjunrmm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zmevcjrx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zcxuuhah.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2alnqybol.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2sfsvoavj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ythhcgbs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xzcwxefk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jtdknijy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wfpwqufw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2unnaawlu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qdtlduvt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2sfmmvhwm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xlamxuov.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wpibrpep.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qynqwqqg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2katnjrqq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxubhyse.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvfnvdas.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suekzcbt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrudzjiy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2qyfskegf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2urvnfrze.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xbljwyiq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bprwdwhd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nzqhgljb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gusscflc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jagksczp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2feaajnra.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2fbysskhk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eqlfpuqh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qjvxdqya.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wrwrladg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gbhqwcwl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kyazofgy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hxcmgnuw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wfpvqqpp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2euafmmmr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2darutyav.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aglaheti.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cgawiplo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aisqzdmb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2lwklapof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aeucnkee.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hmdirzuv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2pewqwvwm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gokmjkvs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2szdiedoc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yehtzmqn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fycnhuge.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gexqompv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucnvlrtq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2heiplxlw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjraxycq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gyzfbiti.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tvbmqnhe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nkxhphwx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ibemidrf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nxppjbyk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fskvhtvg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2gzinrurg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pehzdmrm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2etlawcdy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bedsmbaj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2joogzvif.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bvpbgjmi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fadwvcyd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2omzuwyqr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cdbynvbk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rgbxizku.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vytdrkop.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2rqozeiqm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sbvttivk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xzfqzirk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vihpoyna.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yjzqzzct.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2sypkewlm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gpogfqpj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qzzgaalq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qncvkqio.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rcseysng.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2epxtphti.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dcthrxck.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bayxfphp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2klgkiwse.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2weqcnlvi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fnksknva.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jyykhfyl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbskxmsi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zyncdpwa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uydapuky.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iytaipth.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqnmkmae.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lesgqjdg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2axpkujpq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrgpmwol.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryaoezjc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ptzvoiwe.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mmmzcjxg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjccmdc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lvjrwsmi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2giesbujc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uvhacrkz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vorprgnz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbwnial.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lhhjybba.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dcyxtsyz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2owreijul.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ydbycdcx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcdsorlf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zknwyomg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oqojgqsb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vkkqdxsp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2kqvbeyzr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fqcodraw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hqdocpwn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2rtpixxix.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzxdtxxj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yqmyjynx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tbyclcfq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xdwugqwb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kvdnsdqv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2baetazsq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uwdrobxw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2kyivvyco.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ceqkjrva.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eepmmkhz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gpuqcczk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbrndtif.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iozjujcn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zukfekoe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gkklgfno.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cbxvlrud.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2noogfbdr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2thkvsohi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dujvjpuo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wyubmtck.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzzzgxkd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kmygqefl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2clqrljki.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ztomnjqy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2udgsgrpl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vauozeuu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zmagxdxx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rgswtvlb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vmsgotqy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vhtbdyyy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2euvliygk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nuyhflfy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2nctajrsd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2najgrvyo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zqeqwamj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhxlartt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nfalbaxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2puyfozaq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vwcpaoey.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xdzgllth.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2eutyeylq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlukbqpq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2dzhizadm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hlbcdttm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mlvvnccq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2srrxarpk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xmhdszgk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2racjibpf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2phgfnsrb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2snwtasfd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nashesqx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzvbyoaz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovnzrrng.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2wpojwudd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2pkdxjrof.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2anvyzoxm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2utwdhveo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wbvwmqag.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2otyytjmy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ghswgbkj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2wxomvrxs.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wjxiglzp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kfbsebww.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uvzpwxki.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lnuaebmb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yrjnhgip.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iirrlrgo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2euozcfno.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgprbumo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2njimufvr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ghfntvpl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sslxirjy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kyrqpaqa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jopjrdea.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ckmmcwiz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jzapfdvs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcdlwgpo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyxrpaxb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfqdnppq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ubhmxyzz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2yuypkvam.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2jzpxrrcz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hswpdrjn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2haqmfdom.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wljclrdu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvoffknx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pdnwtksw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkcajymd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2esspjlcv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hyvmerdn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2sjwyqrqz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pbwpopju.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ljppklik.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2oqgnleco.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fpttwqcm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eievgtni.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lauvfezo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rovfgtjh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hotfonbl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xfjrwjzf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zbokuxsz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2kahuoooj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2linfkylm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebaijndm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlvxhixg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2qaelgqxd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gofzuour.html


<!-- 参考信息 -->