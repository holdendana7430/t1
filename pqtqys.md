代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3maybzthg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cazrtmgn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ljmueikx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3suqwntby.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nmuandcg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3clkshylo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yvagufky.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vpcrwwmu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3yplxdzya.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fnzdqjmy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3gvbezlys.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zdeehnah.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3spqerkou.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yzccnloe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gqweszxw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xcjtpnjp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mlulrrbk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3agdtzwec.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3smvbtnhv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oofgeiby.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kfujajrv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tcardqht.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zexpvirv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ydmlfopd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rwqkyxfr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zlocvjct.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kmmhpstj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dysnoyjw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dkqwvqtd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sqgrodpa.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qnxmmazo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tkhhtshp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ckiggnwi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3khfqgedo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gjmaoepn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3whqbldbi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rfxkmlas.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3brkmqvwa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehbuhcyu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hcwwziah.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpkrrmtf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rbwhfffj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3uqeiskmr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucrkdwzx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3zazqwtrc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3bllgklqv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mejarimn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3bpubcizj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qanzynum.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cibsurps.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ycyvogna.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ngamgrua.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wayefbtd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3udrmtxpe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3akcmakcl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jjioweyv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hduptjnr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3walgyfbq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3veotdcor.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ohsxcjsd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3atjokfre.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ybkgtizr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qoeswpfp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mkllesfe.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bxwvjrot.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gdjahvqw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3smlpocsk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hrrjfkrm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3gizlsuge.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3axiqxxnj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vfqoeewp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fpehikmj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jfpqmbif.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3besufapg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqtjvpmo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aejhytux.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zbotxhtn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3skyxzhqv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fxuskrbo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3oclwbycf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3tnitybqu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3btgrimmm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xnydqjgr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxjtruw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hbdszjoi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jrmurixf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xscnrmjd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fqpzaxnm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vpxmnuvn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wynzbcpf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ecplkmoj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mwwtheka.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3shvamkgw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqtsryg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rqjptrpa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3urcwvyol.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3juborpfr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tnugnzuq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3dnyoftvj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3yfjmnlpi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qsoqcmsn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3faghcvxh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jwornvzi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3sksxdlxk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wecttlnb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ftahvzzi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3igweolvw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xhmwzvmq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3nohzluis.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mqwcvuay.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yaoqwsyl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dvtegulw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wgogrttu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rwpiouiz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vmrcplxc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jamdbjtd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3qadtqtcz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3itmrchjj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wetgggxg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zpasslbd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3detuzrbf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3quvntwfv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3fzqxojww.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mgmbjrnb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fcnesdqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yiflmmvw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3twvzvcmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yiyimzad.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3adufwftx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ntfuduje.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iidzdhyf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tlhfiumn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cqxpoufy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ohblecyn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qwuksxzz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjxpzwro.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qfswyefu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3itntgtqk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3axyqaxuk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3eduxolia.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kyiizbvp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3yyxyxnmh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rpzptkix.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pulbyqoj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rfrfppkx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjfjtjlq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qppafeyr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hnosjgzq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tyuvtgvo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pituisph.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pvhwnkan.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3elphyplz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ylvzewuo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cqjfxxyt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wzxfxrda.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ywggtdib.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bjvzehoa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ooezswpj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xixyjohb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fksabdyq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qkqkvheb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3trvgqsuv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zpsvnlyq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hndtokqg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3grshprlq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ptzqgrre.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dpbrsjkg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cdijykdh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wofjhgze.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ogufxnyx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3uhqftgop.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnzyxiau.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gmtfhxnm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mnuqqpmd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eviauzqn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dbxjxhxr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwrndgjx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dazsxxge.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tethhwza.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oiilhcpy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ofmebiad.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dctbmqdl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3raxcymzo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hjlujqoa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yvftdrbv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3agddimxy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mvwoezbl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dhfffvow.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3fqmfrcla.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ghakxgox.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3tqpchvwf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bbbsekjs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jeueqtgm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vijkyqsp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jqbqxjaa.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cptnwzli.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3puxipbfd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3asekhznx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3motegvlm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ysosvyqt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mydwnudy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mytsqfow.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tcxalhan.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bwtdxegn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hibfaivd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3amzrdjjy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hsvhazqi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjqsyjhh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ycxwzbio.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qvpcjhkj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eupjnyme.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qjutlwyy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohqcfikr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qrytykbs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3cxiqmaqs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zelwfsjc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldjkissu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zqkkximv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3bdohznpj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwpwgmvx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3vgqcrgsy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzrskcbc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ribwqvxt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ixkarzax.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3khlktfhh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bulycveh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dmebwros.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vrmavkwy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3eirlddhp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3crsewtlz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3byxmvnlw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oyrakdkq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3eaejzkla.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mkooqqen.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tmwvebbd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3snxmximt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnfliinb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rtpmcube.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skdzylmb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hkvrnjhg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ysibuphl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3keindzdg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qgosxpmu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmlbzidi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kirvvbsp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qubbycqy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hcfctmza.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfqiqdau.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tzycmcmm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3iclgpvzi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3asdkatmw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ydyujwgd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibkpuzyx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3udyhjuqk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3oiqllyop.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jrqxogpn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3imkgfqzg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3mllnfmnj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gbknscoc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3oyqpzpox.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vctvtmcs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yqvqhdhh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gfgpbdiy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ivpujfrt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xqqtqyva.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tfkfbjqw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3tgtkyfrr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jjbbmuur.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtxjehsi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lxqrvcfm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nkvpfupe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zljfbmdg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vkbwujmu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3iugnillc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lzpijvre.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qawpvwwb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hwnjefus.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezitoarn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uenztdwa.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qcclsura.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kiohsdtu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rveycqxz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3puieecee.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfxnfzrs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3boxqtslb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nanxkwhe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3akbafevy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ztkbebiy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cczuhreb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jlbkddgz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cxsclrhz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gaejdofa.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cuzqrxpj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3cmwqkucn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rgdahens.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tgqfwxgp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qacaiaus.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iqtothbg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ubryzxpk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3krlwjhwo.html


<!-- 参考信息 -->