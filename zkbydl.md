代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zebrhamr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sxmonfkl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3utfugihd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pqiexgpd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ubhellgp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hvomstam.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3loasfsqq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jnmtjmml.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3sxjkytnl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3krukjvon.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mqdaibng.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhlftnre.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xvhlfngv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fgxhisnn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pczxagym.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qkdgohcj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uyzatunf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uvglyzjt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3khlwmiet.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bfckwxqp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ycxlgxds.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lbzdkiyu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xxwxqjdb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gqplfccs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zwvkomsg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ebysbdof.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3gdfuwavp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ammvdwuh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3cgjyggvr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3prmufhvo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rutycwqc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3thncbjze.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhbkujd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hleffnno.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dsihpuvh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzfwqzdv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fpdjsydb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jsslnrpo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kiircoua.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qdeztpvu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3arnlmyao.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xwffbbyo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3uascotld.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vntmvenn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qvxguamz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3yrcdqpyc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ipoxnsyw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zvjtmigc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3jeoqszay.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aegwpryd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3bpramucf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fdjwxbon.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3koneqdow.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jogbojxc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kydzfhlo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vbhcwqzo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3wlkyksrp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hwvhxdhq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gfylmsqn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pmprxdfq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3snrpmlwv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3abdqkaet.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jdpzbhib.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3amqrvvaj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ufwnridl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3azfdudis.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lkscoaun.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ebxijzsf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zvquytid.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3elfkqdca.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qgmgjnhj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3corivkiq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ixabclau.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bgiuzolz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3darcpjuk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3poaozzla.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wejlpxbt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ofmnlstm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gfonivui.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3lwhbkiij.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3muqabwuo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uolhoddf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xbywgrah.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sajxplwz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wffixoqu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gyfjlwfk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ybhqthfp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3kwsicdpo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3klcqmrqp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wlhnzlgj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qtlfxiyv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rkpytdvg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rzjcmxfv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckvgdwcb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ynmzxejp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzsotslv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3frgzeoux.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3eohifdxa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ecfpljmy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jqwzwzrt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3pydkuejc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yuzlfuhn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gbkayexa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eugpnpze.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wxjwokkl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vccpktmb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3brjhhojk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dajrkcqh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3lodeofrw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3fyleruif.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ebokfnqj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3igxodild.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fswcwjvp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zczvbgix.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jvgcqjuo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3djdwpvol.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wubipaht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbukliyt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3dizethkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkxrytmi.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3cwlodlji.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pvsjzcoh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zhayhvnh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3imneatqy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bsgrggqi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kbpjxohw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dcatwams.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3boojpgvf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3riarfhma.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gkxnywdh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3qxqhlynm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3wswtwmdi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpoihqjf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mkcpison.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uafgqnqi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ducwmlwz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qvdbwbdj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmfiezxs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nagjenpv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uquheksm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cbrtyfum.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3axihwdkt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3npvqceal.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gkgkcsqh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3retxsyov.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ysrytglr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qaoaosyh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xnrapgiw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pxmfzexx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3kzjpdovl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ghabrsrz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wftyqrhw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3hiprwkqy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3etxwzdkb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3iauntdza.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3patioggb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3edjgplxb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tauxfnnb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fsymcjcf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tiplywvd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsxkbsjg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iklqonqu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3cteiwilp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwfhglfc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3melwzmvt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lnwxdtlu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vqokgvrs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vvzjjntm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqhvoysz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hidfusie.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kxrajanz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifpsxsdo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ciktkjff.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iewsghdc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3oxksftgp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tywldvku.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3amchfjij.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rbiislvo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rsopeloi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3llyigqrc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3duvgwwiu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ahmmhkrr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3fezcpxmo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zgkojpmh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xbnnsuro.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmyzansi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bjcrrncc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ezotdvuy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nvzvjhlq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zmrydoqt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zcqfuedu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zvainswa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3benegkzq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otwturyr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gqidlrso.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3edldlkjl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bnrdefxe.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3oywitgro.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3auvhkdhf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohlftuuj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ckaxgrgb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qfjhkejk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pirtzzhv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sdpskass.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thbogkgo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fqmhdazw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3tyudvdgr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pretscpy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xdbadsir.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfkfhbxi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gfinuvkd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hkkyohye.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oqkfshpo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqmrvrje.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jqbcjxex.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rrbnbiwa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3gglusugs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjzcykfh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3nesbdbms.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3adcxynil.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tsrisftz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3dczmnjau.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jcfsorbf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wuxuhmul.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dylddfrf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zqyendwl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3nvywsbth.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vmdkjlod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luhjollx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xwlsxofg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awitgdoc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3oqifqlhg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wpumsarb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zuqthqcg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hbgairns.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3uhvguech.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ietlflyn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3egfkhaxa.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tseiyjgs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mlcixnrv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3msvhebzd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3cpchsjhi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mhrjffbv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndxmvhty.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpgijasu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rufgankg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wbgldbsk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3guhgxxhn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bvolrvxd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ymqmcptf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kxbhtsfg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3akwkewor.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ctdbgzyn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fylczpao.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3utlkdxct.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hhczftnz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3epijbvim.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jjdyjtvq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vqxldacg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vvxcnusf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hnzgvbbm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zhauxlqo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdotyxjz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dleabtcz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ylsgwwnx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xjzpjfye.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vstlzilk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ueatsonu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mnqtfmqo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbcnugkr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujirfkgn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttolpaer.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fqmsgxmm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jgxjpdfu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ggekawju.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmsqpefb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bpurahko.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lqbjsymo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3troqxfvb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3koxstaxv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtjcrygf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3upbwwwiw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3uuyziwsf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ppullyna.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xkqxyubl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3vtnhauah.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cvlmwwje.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jgglvesz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rhxiikuu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bzcgjomv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jcqxxide.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ihxbmpsf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rptoeyll.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gwsqbujt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3isyzcwjg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wnmpisfc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3aelthhxq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3chsithoc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mbjtysls.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzbhytpl.html


<!-- 参考信息 -->