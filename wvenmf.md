代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2lotpmnea.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ozniwsln.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rfeymqgy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fbsdiyuw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkvjtbqd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gxferjdi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jsnijyat.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2isshqkwi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uzcknhoa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2utibhbgv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cknuszwt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uiurcuzn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cagblaxv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qlfrzhfd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wsjojjew.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fpjfbcxn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ihrskqtg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yysbxsyo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rryvnuoe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nekvofxm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wookrgdb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2tygyenfy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lawiadca.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2szwomcff.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cavszlvu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2orgfeqff.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xnmqgbqj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2eussuxtt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cjydtghe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2njrbhfkl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2iifhmifc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uqeqilin.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hdveshxu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2enpzrdtz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mtasaxvn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2tiojjien.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rcifrqzd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2csslvmax.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dojvopto.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2iqlfokvk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xvgntsqk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tdxtkuvv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmujskvm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmlevejm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ighwptjf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xcayofpp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nlfjjekn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xbccpdew.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2spepszra.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kghaypid.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cwkkudsn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2iurqeutg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2clqmyknw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2souwhagu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ntsthydx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vgkukopd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2svojaale.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vaxnfnyp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ohdvbyod.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gpnshnle.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gpgphlgb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2oqthlzur.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2owcwklip.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2xzjsjfon.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwahzslu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pxjgwstv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fhwnfndw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2iwyocpni.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2cwnkobdd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2btewqzff.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tvcyzugx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xuuaqvlg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nyobwwdj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2edmggioh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2dcypvyey.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2slbazihw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2grlkppvl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rosxehsr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzhdrioa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wxijqzym.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfjcmijn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2cgkmnpvs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ecbfered.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2cokzbgvw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2khezslvt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2eahprfhq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mjfgolrl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lmrcseig.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wpskugqt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2akahjdrp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2odyghvek.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dtmnjpzg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ljtjtqhc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vullbfxi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wrxtvckj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2acgbjspp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tlrttpnn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2udomglqj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2srysapzk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zufexnzq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jedrguou.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gqadnlgn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2adfboahu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2lfibjqhh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2srbuyurk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugezmube.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbrhqbxy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cembofxb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mflnkbed.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2crvzmezx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eigzmfvd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xyuzdhpt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2guhedetm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rwwlxuho.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iasdmhra.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hyoedmxz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ufsnhsqe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wjzlatzg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aanfhbjb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ssxicaii.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2sqoweqkt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2fgbjseok.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pdpbkknl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yybevdic.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cyxyenvk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wzfppnoh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2iwgksvqo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2alrrxqad.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kfpuhbxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myuxjrqx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2nvnqfctt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avgwchrg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yfpjwmlp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ebldhtou.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iwiokxjp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wijbiiiq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kovfmubv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zdibixia.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tnzcmrkn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yzqjfkie.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bppnxkrp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2orqnpbqf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xkpkuofy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2atexezjj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofsxofps.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rkczggcf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wwaxngvo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yxyrkiql.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kotjzwwg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2nucplflb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2upzjflyg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2eoxrbfuj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2opsqwmzh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rgrertsg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hjikinsc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2unbvozlw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2roaawzaw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ijuhyhtr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tlhqryfy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nfthynex.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2teswlbkm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2eqeiwrkt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2inautmww.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hvatfsgj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ztwqvcqq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oajymtqr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2gsxuliun.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2yoxytsel.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bdpwtlso.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2snmlurnm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zkgcvydi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxtdtast.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdiifwya.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hqatspus.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mhmwymxk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ommymglr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqarzwvs.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2vgzotplx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyuvvgba.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dixhzqci.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmztvfic.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlyvcirr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yuxggyvy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjnghkvc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwcrykph.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cnftqtvf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2yjpglyxd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vhehcyfp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mfsajrpg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nbbvetsj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yamwbxdy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2hkhalxtk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2skpgewqc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2buokothv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dqdqtpmm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2niuseeef.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2pjgicfgj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rimhxnbd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tdetnygs.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ophsrjfy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dwtslpek.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2nlwfirpn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bxzowiyh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qsoejjgf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2npghhkos.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rnbkkfyx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kaultmtg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xqcpweaq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ltpikhlj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xetjemub.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wxdphyky.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzpqqnzc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qsmjekcw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hbvlyngq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sketsfzy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qqptfpsb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrhmugeo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afjcedxa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2yaxhmnsa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjolwpay.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqvvyavx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lykqeumg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfjbdjff.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rckqrktt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2voqnaaiy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lpatyxoa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2krumrcmm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qmetofis.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2pexwrnrt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhfurzdi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qkccpfbf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2sidsyxwd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2hjxmexhi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2iymcyfzn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2unymbcrn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kigutcvf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dulqrkgk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gglqvlbe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2oajismbn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ozxqepqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pumdduuo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qyztvejc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otihxbgb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2sjkhauid.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jjtfryng.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dndrlikp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ditpfwxy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cmyixlcy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmdytsjx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2geksueab.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jqzzwgpa.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwccrskp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2alhzthby.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2eyuzxiaa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dffvlijx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rxahancs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2buryyjwd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pdcrytks.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lpeavkhz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ykqwasad.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lafxbecm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2dspswyhy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2moodfgcy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2skktcrik.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lzmunuyb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hvemnphn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xlubivjx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2iklxxguq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dmvvhyzz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kbyovema.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tyhaeonh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zawfppez.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwimgkmg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyvzxopj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rbzshjhi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwgebflw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fhinzlka.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mrkbmswz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2knxdbgza.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wexrtwca.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2trbpkqxf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbrmsdbh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiujuruy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlqyzook.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2avvyibai.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2toyecutz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2intbikji.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmuvekxd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2yvozwdli.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2tizxvnva.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nmrkpsxp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrremxeh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mapiyqjy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sftuwfll.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nqutyvpz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvvaoinc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zunirgfz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ltmlhxmd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xczdceaj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zsvjsshx.html


<!-- 参考信息 -->