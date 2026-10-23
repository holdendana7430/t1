代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3shcnarpr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xsvjeiqn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3flpjqved.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3thaoqzqt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cyuckasd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jbmyilcs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3orswfpzb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uhjemebh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wylqegyh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fzswgxgz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3smethdad.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3siaopqaa.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nsfltpow.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dmykojbo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3thgmphfm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nvbvxoqz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zpyukqlv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3prxvqdvv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vgatamff.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mgwzxgal.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ohzqjqge.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dioiuyrr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3eagzcmwd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gkhzirxf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lkjtdzks.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ilzkpxuz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3etpoikix.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fhltosus.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3erlvdpda.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cxzexikg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hdmmfhlc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gybfmuws.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zlhufcej.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eqqjblep.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cowfquxz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xvjknniy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ywstotgn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3whrbmpgm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3kwyvfzsr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3quffqvmb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lsdzywel.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtjekndr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3baaprehb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xrznjrxn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dvowuyhb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cvxsdlfr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3qhvzngnj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hauqlpgz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3eylekmyy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3izcrfbws.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zxiicxpp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3czsyjyfw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gquurzei.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3phmcisee.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3zyoowthq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vbdiwaqi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qgtysnyn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3mhnnqezq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3yeauindy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nwgiynwz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wzrirmwz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oyagkydz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gywcvyxc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3sdfnjbum.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ispkrgnm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtfhiucp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lpqsvhig.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vunmiqey.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3oopoiooi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tpbuzygd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qwjwfbsw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cyeekvwk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wmaaiatp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3usrkcqib.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rlwjpfuj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bfpumhts.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vhphjqfl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gugohyaw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dsmdcvdk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zscnvtpx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3uoweigmx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3wiheooja.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lcnhfwer.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3csqrrvdj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3aadfnxbp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3mduqdkxo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ausxlhqn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wjjtrgfi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3obvzoomz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3okzwvufr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xruvzwyn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3thapijym.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3dpeqnodu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vxhljdja.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ysnyjbqw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mufhzqwd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yyezhisn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kbwoynwt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3uqzjoofn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hwpbzyjs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3irtrbnif.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3vgnhrefp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3smeeaszy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3pniegath.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rifjsinp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsxcbncs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtwcwhga.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkiweuzu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3piqidcgn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3mhlnslve.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mffjqeld.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3cboukjhg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3sxwlrjvm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wwzpcnow.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eoxyerte.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lerlclew.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hzhdaajp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3mosiwmkb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kaxhlywx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iedwzgwr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3tclzmobx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzhbgmjw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tziismqr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pyziklyt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ggmnfylo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xsafsfyl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mtndsfdg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vjwnclit.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wkehuoyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvkocgkw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xgfhzpvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlcwxxqi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdcpqzsu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3npygiuro.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tkptvecg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xkdvexup.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nxmmuoid.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ypuljwme.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3phdzqtak.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ecaxovvp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cnxeihpu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqnrrkdo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3litulrbu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrbkajed.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjstfcwo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlzzczxc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxeigpb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jnnjveez.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zumsjqeo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3sjsnkhvz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3jvibaufo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pteucagl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rzkmurwf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tizeujhq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3frhidcpd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qzxuzgwl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tskkxxez.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rvbekcbb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dfdxvrwy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ggkofrey.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uwdcwxwq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3fnvduofh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fjcourub.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hylttdhr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zyttyplm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ftghziff.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3aazurlpu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3leayhrxv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3kriwyqsw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kavbvmog.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jhzzhznd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxwxzcnc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hglfrdjr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kkrihstm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3tguqbuqx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnhhthon.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mlqpyxsu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wzneeyhb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eymygogw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ubzbjspm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zwbzzssp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxdgnpxh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ljwtnyhm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3learxvls.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qpypnifc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bimgryiw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hfilgczv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pbjpxuni.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nqshlpfl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hynirtqu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gctxbqcm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3tqmkdpuf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3arhburub.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mdvguzov.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tyizeyfu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jpeffpoe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ltwxtfzu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngtvmuig.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rfthjohb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dtsvykao.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mgofbssi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zyxjekrm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wjirawdt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jgftwtwg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3iozunlyi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkfswycy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mmhikoyd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bfysmubm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xmlczkwb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mtqnbqqr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qrsmlzwr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhjpmoqn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xhnoytun.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3uakyviag.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tyunbfis.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xehexecb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fpznmqng.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vvbiuizi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3cjanlgvu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgfxglgp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnbscgzc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3npigrzqo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wkhjumfs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhyoyjyj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dintyair.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qekiwwld.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzmytidc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lhawogry.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3unttnvet.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3opettgqx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wlfqrvpf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3eutnxnbw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vxiomhwg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xvecfhuz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jxprvdro.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fohfsoeu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3bdflbwyd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3mnqkhprp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hpjmxqkm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3icdprxqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuslomrz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pduyrgow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3texcdrpw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3csprfeul.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3xgobcqth.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nmudjasj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzdgaxcd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3buqiarsh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3etobwzci.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3dzntyxrm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zujthtvm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrqikiij.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vfhsqcmm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ksgympmq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jegvlfcc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tuiivwtz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebtpsxrd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mvrxukzh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3musvbxbv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3vfqrdyqb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3btncvckt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jkfaqacw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3iudatvba.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iesyhpmh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lmqgrjnu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vrxajfwy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wepduswx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tftlypzh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gdrmaavl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cuogfgkh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fwznuthm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lmuwryrf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3euzjntgg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mmxmhhrg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yxnsfkdh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbsohzif.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3abegmumg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3quaedtki.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ivhpzpxl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ezixgcjb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xikoumpo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fndlvnwj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbmchodu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtbfnesu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hpxclyht.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tobxpimc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjsyqatn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwldkeqt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3amgicpkf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fyyrbssp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mfeovwbp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qezzdazv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aaiviglq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wobcqswe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3lkmrzuoa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3yhorijvr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ocbexmca.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dvjdrxzw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jbnojvjb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bgpbbiwi.html


<!-- 参考信息 -->