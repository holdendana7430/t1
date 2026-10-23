代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3mmuhigym.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cztzosis.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qthuezqa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3stmmzlas.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gqyejfpp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qhiymlfl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pycfqcrb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xkxlmgat.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hdcmgrpj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yrcucqbk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3oxtixzfb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zzvmgcvr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wbmmjqie.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wdufbqwa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iztoaekz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kwgenitv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3eeankbbj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3shkcaeug.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vzxsxyht.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vdpyniqz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rycrbytz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lasvpujw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3roijmufz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3oudbfdiz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3owofupmg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kshrwzta.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3uoevtjnk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vmlxxlui.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3votkvwxn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3aazcdezp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cbuegwbc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3bqqndzpg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pdghgplb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3inzjairi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3awqxiqvc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3syppbbzu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3vlhfoldj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3nczntxyl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssqvjkzq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ubobkzpa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3epncilsh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rnmknvzm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cydrskgs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nfhlpffb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jxtrwtls.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rtjksqtz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yewqnpug.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3iovjsmis.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nbfosauy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xloqkhig.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3revkzylr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3eyszkzdv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ibxmfssa.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xdaqjwyd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nrkrtapb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cpzixphx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xxgsivor.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qkrvwhyh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3oiniyxps.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3onodrfkl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lcynbllz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fuizizfv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ibhnzwrs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3thywgoqi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ullwnmeh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sihvronq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zygelwad.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jievqtwy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3tupoamxa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xbhugxsu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gdvvovro.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3zduktcoo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3psmeatmo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3blquztci.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjlzqvyj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkgmcvvg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kywfopgq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nbkygthb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sbmnyzte.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vlussddh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3kgkhqdgr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3klsqjqes.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bwmoaoii.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oxxbeliy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3azwqwouy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xlnndtej.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oxvjtwpl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gqdxyitm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3crmesdng.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3edoexics.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xxibpztt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wbuzsfta.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nvknnqau.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ccpmseux.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cttlpcni.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qydtilws.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wypjktcw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3yiqmkqtp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zhgjcqqq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3uczlvmfy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3maosxyhu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hlyfzbgt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pnvecpco.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qprwbloe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbfpmsto.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3uwmismea.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvxvyexc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3hjyfynuw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3fpscbyym.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vezjjzll.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3amnkmimw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cqykrjjy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jnitkiul.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3joumdcfw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wptkbvtb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mkhwjxib.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3wfghsert.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3inffbver.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fbkedwbe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ztcjjqcy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lthcvlbe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dbfvyklv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3iypsdzqo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mwoiqoci.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ayklafix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgiysuhb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jscofbxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wthcqjiu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjbjsafc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vatlbdmk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uadksmdc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qlybcqkz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3inngwurh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xwtezpne.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ydqiunsz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxdyaczs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yoereytu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3mvapaehg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3whbankcx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3airfizqv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjxzrntc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rwmudmjd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cyryerzc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3uojqpfvp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ffpzwvvb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcpuvnuz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3iepwsfac.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uivsfagd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3llbjnvlv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rhxkaorq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yuocxgxt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jcaaqpvm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ouwvxuts.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dnkhjrwp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sfqlqnxe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3agfxlpbv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ysctxghg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fgpffscr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tljmpmuv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qtqeosjk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3raglonwu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dloqpjkb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3cmnpsqgl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zazmkeoj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fruxxbrn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lygktbol.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dyksssij.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxwjozlx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqlzsjjy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3scbgelwc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3akurjahp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdhvpebi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wbnzsanp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfmhxgjw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnysqjow.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3umzbdwwn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsextxkg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kgugqazh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gomgapbi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nxqkwynm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfqnfwhe.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yldhxjtn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ouswbhsj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bhehlkaq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dousgxmr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tkewlsud.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cwalchlc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3almmgwrn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3cxqltshd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jpnkuemg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3eklevsfp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vjupalap.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ehkknkug.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksczqmvr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3juorugzb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ssimbbew.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wftnybyv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uiofgpzj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ftrwdrdt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nsqsjlrt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3msywfual.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nccnivfy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3svtjvsom.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3oqvudyfw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bulfqult.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3snophhmq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rgydfhnj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqyugmfc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ndwexqww.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wluwtjsr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgqmpypx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mhdndgfm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqkmvbzz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vuwxtnxe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mgopnlze.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gutiukre.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdayzlgx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jsaswrgl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hheodvqw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nailqhml.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tezbulxk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqgmyaco.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmkkfcat.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hoxqmblf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jwcgcupa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdfrdzoq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3daklpxmb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3igtrwmue.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3nkdozmkt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3hlaiszfj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fjdakmuh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3cqvwxpil.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mgmtzghb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3lcqsaofq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3swgazxip.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bcmcrkhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yswopovt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3sxmgckkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtxwlqbk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3usczezqj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3gkxtqrhf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkadqszj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ktyqhqbm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rswqgdsv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oananbej.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tewxxeui.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mctxhflk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cowkmvkn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pfbanuju.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xhzgsjnq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yoeurvnc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdjgwlyy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3nnzetela.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zsjnzybd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wktettki.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gorttmuj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnkgmnve.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pqingspz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hkfokelt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vrkorvhc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zvjidozt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kfploibx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mqlwfeee.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3engiouha.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dcpeqwjp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mvfooblb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3efjjtlsw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tytjmgev.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdtwoseq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfylxywc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3scgavpvj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jxxbsekz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gwlzssjz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3otbrvqlk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ftluodwm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vhtwxwtq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tyolgewh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3winmdgoa.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kccqzrsv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xjlnxgpa.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqklhbpt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3spjidpub.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ebfbmsvn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yltbjezt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ufssfmyo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wfoujkqo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3szzkgqyw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlzlngwu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ithhtrms.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggkimwpj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ljaipyeh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wehokdgf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cirlncnu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3kwautagb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3blmyesqb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gowgwtuw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vjmqahcf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3btrazvyy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3caqyzfbr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rbmwuwah.html


<!-- 参考信息 -->