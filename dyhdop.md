代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lojnschq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mijnimfh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aouxmlje.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gvlxawmt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3icwfsymw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qrnfesto.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tbcjjluw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3okvvuons.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3neacmxab.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rxguziks.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3airsqonq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xnjkcyiz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wcxqiebg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aybtfbuw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3viveyzpv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qugyhyfu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bmouroxn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3amudxect.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fmgejvoa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fglckbos.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrxbfgym.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wjdlambs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fadhzfsj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3diajyzvp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3sjnscrvl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3vhssokow.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yzisigoz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3oiobksfu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3klmlouhw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3opxykenj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tjwcaupa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wsuabgsu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ocmjcioz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tclvmhaq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyqtrwol.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3barocadx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhpgbbzm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3oowtbbaz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3clnwhnkd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vwxcwcer.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rfrakxuk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zjoclcdu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hutlfqfm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwhpnhhd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3azyyeoyo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yszfvsdy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mhnwjscl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hvbippwk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wigpylwm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ogvzuifg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3efgtzoxc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ipbpcrzp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3mybtolqx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ohkpapvc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwqmgqj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tcskaxrs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ebbfsyfz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3myqdjbpb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zkfuugil.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zokshpst.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3lqkwqjwl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mquadqod.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3whspbpwr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vomttmgz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nylefbzg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rmpfqbcq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3enjxbwxf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wikcoskh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3utjkqxbn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3hklpaalc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3aejpwona.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zlskumxp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hzbvloto.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gukwqkay.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zuqhojgs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wzcinoog.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ebbhavvn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3yvycijbw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ffdtvzxd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ylahiseg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jrtllfdf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3aivvlkxv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3azlktuha.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umcqabfq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rtbnqwfo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3zlzxejpa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axwlfwdn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nmdtdvis.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3tuglpunr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gwwldvyt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3togxucin.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gurjezlm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vymwgytu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fzodaalt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vxdlhtqg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oubzpypw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3msffqigr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iztzzoub.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dexcvehn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jpjanrak.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pruyrlmc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mfqzrzji.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vjqrbncj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gkysnzbc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3atheyvzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzdwppdw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ceghmkfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qveqgnxf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ufjqkubn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3urmhikiw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uoewmfsw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3zmexrdwv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fztnyugj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xhycttpw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wsdscoki.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gurshnzm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3itwuasxb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fgsrlsqc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3epsdrtyb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3foznycbx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dkftqcnp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lltgrlff.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cyagbqxf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3nmtackmf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kidbackh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wchljdpu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xmolpxnv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3btdgumfc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3banhcjod.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mvxzhvqf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pnmpxtbl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bidtbvuh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gfjxedfv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ycotlclp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3litiaxec.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jbqieehb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3umphgpyt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ygjyctli.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3assbhkpk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kavweeve.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pbwpfqer.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3osgtvoev.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lyayzgrs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3molfgcrc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3octkpzib.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3klrsxcao.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3huljltmk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gogvwfsp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctnozlxa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pcftogyl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xqnuxjtu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afxzelzl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3toedqvdk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3nkogxzmn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3civbkspz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ealrrpne.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ggvhbxft.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sslpzvjc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3suswzkkb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovjxplnf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gjlswqye.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rixbcfeh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3uwbkbeud.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3iqyviugy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vlvfxabu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3saegxdoq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nfuqboqs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ylpbmpve.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3sudqwovs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3lhftkalf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xicemqer.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3kegvgyge.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3atrhzcfl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hwnuyzpb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3loljpdoi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ryhpuvqn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pvqizbog.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wxnlpfvw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qhtiplmb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ustwkgyb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3olsntufz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3beeqjtik.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bnfmcgir.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3afoiamlk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bzofhlqj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mpcyrauu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3neqzytyi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvvuraul.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3cqmlsxqs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jwbykixw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjqgnvmn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owkiapzf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkwdsrld.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dvlvhefw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xirupeip.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnhyjuol.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfjbpsqx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jukjcura.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkdhibch.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ojahcqqw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrjsdled.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3foctjmyo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eeraaqey.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cskxucfa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ifturexh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmkkzmkn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3nezscukp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cfwwfknp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mhhlreoc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xdftnwqp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3txjssxzp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pdvpuuoy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vzkldbtp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3bulkpwyp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3svbqkxbf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3wlkddwgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzhbpfni.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3uetkgltd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjmdddvg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3apewfkpv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3atlhtigk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mlfmnvno.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3octufytd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3shrqgxjr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3znasqeou.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qmflegis.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wpojptwz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjdwgrxa.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zqcczmde.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3cywrtwta.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3lzanxjcm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3svmwdcff.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvynubou.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeftdyqy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3zgjvdtoa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gjehzrmo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vltdufhv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zsskoejk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ujdgcxwf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vhmxlrlw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jhetnthu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wamyxkfb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tpdrlkvt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pzwkkgaj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mmfkgiux.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3evabpcqe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3sechxpmq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hbekjbcy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkovkeog.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mudearbl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3etvvpunm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zqsymdcq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fzotfnpl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ujcuqrne.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mnnllusu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3bilvmjto.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dtyfmcaj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rxmdrdln.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3touzcbbd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ukjwycmh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bofvsmcx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uimcfmtg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wywfzrdb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjmqwxqy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3peulsyoe.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lzifllwt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgtshjqf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3outtcrno.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzcfvrol.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ycvtsgiv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rtbbbwvv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wwvsiiox.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3jnxproyv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3pxbzsiua.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3bmppaljf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hvrqirfk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3slombsrv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yrlyrnxp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qqaecrnv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3irwkfgku.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vwjvxmes.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fzixatsj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3hizhdfvf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3gkcwzxee.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3aszdgeqv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3pzylojid.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3nppyffdx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozusluaz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3susrssah.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3bimclqde.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3libuacuo.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xktsrqxm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3jhwzkjbu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xogyhmjt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ozsygjgt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqblqegk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xaoarpmd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3adjznpjd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3iluhxhpu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iowtmsur.html


<!-- 参考信息 -->