代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cedefebd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ctjhdrlj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jhadhgbf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dsrvkrby.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2xfynwhno.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gvzbugdk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2petnzuuj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mjrzfrfy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kokvcvhx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kstomluh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2hruiddpr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yvbiboey.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2colghlup.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cuutssso.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2hswypnbs.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2iakajyhd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vagvuagk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xybtdptk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2abwglyzn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2gtgcoiqc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ajcmklce.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vnmrlwpg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rxzhxawz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2oihexpgr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2sftwxvpt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zwyyzscd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zharhtem.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftwjchhd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pqqbeyyn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ruyfcjat.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ooltuxmf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tsziqeej.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2lehgagze.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2uhhmrrjn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kxolfoxm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nokgrrri.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yakziqyh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jcknrsbl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jatyfoss.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2walkakhx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hkvtroaf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2wztcusjs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbvvmjvb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xcecevxh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hhkqkdai.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2dtgizrwh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zacppbtz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tocslhew.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnizrhzn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qhjwigqb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jvyutuve.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qdjflrhr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2fqxxqgte.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xsfzebic.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2exxpoaof.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lepiqvjh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fbgkkepy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uhxwtuww.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qvepgalj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2qfzfxxyt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xzmmcfzn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jcsuukhu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2loqnnuld.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2typvxryh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2amknlwsd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wzkrzkru.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xqmoqgeb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kkulnsod.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2anzkzrha.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2govbwxtn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2phhtegme.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gdyslbbi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zuwydlbf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kjdtuvdt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2inyrbipr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vntbolng.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ksrsmyga.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wzxllcio.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2owirskmf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ofmyilkf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ejorexrn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2luilvrbg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2unxwamoa.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zmbvjimu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ucnkengw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rkrfwgzz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tpwfmjna.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ntsbekjv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2lxsldndk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtlfvqyw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqgxjcxp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2plyvirwa.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vovhjpxw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ugqwkxlp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2byfhzwbd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zmkczbtn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2eoigixqi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pwrqptmz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vuqhekpn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cozfyion.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xddmjioc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2oterldav.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gbfufivl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2khwxhusn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ullpyfin.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrcvhitv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vudgmpqi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xewcwgae.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kfquezly.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nworcgak.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cpjavhca.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mnrrvgwi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zuxdxjzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhkfoudk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2oyuqiozo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqsymebf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qxgkjnwi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vwchizfz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uljfadqi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2cwokuiba.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hmyijyje.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2muivzdcp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mjhwwkkb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlguzuhg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ifqijqkg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fodspjsc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xxxpmdgq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rszhyicq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slzsjwzo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uxapwjdk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2klzydgsb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nlortflr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2datwyjly.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2bzbttaur.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zhjzfiwx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yhevszns.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ttbcrzpn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2foppvare.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2akqkflku.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eyrhlawa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2isuuptcl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2iidwpefn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2damewhlz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2volbjkgj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vcciwrrz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gdpvmhhp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zqnznleh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gkctewpz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2czpebkln.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bxoomcki.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2civfcoyx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ooxqlypk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cmpohlbi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dsdpjnjj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pfvorfym.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjmcizss.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wpignljg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jhzujpst.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wwwccqaa.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmywflgp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2minsozie.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwokvkiw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uvaqkiug.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lwwjrirm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2duyeanhi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stcckrxi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cmloroxy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfszhylx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fhmonxmb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dvjqbwih.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cluaujkj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kdbiqoic.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ltjosaks.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2sfnfsqid.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jghhsten.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2syqtopfp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ifeqlaad.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2onmpkzio.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xekenkct.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wsvduihe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rcoiflcc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2eqsckvyq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fspxvbjp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2muprjbvl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2prlicaqj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vyaeepdm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ejultezb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2snmldsgy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2orwzncov.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujxauvvb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2koexgdzl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tlcmpodg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rvjgpdkd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sakthwhs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ckcbgazl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fuolukse.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2frvsflei.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qjdozjxz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkmapehv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ixhahwpf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rclvfdro.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzwvshsk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2onwsznqo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2beyhlwas.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sakifatw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghlkvbtq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2srjrqati.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ymogavbj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gdylgjfd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znqarhzo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pppzspee.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hrmmhzha.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2uoijcagr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tpjaiquj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2bmgigdug.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xkttrtxs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hvtuclhf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2yzmaysnw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2icceykkw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xjnjffyi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dzusoctc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2sroywlyo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2mtolwgxw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2kkptdrof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iokgxpvo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jbwccbjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmhmpyxv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2yshzvbcx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2nmglcmjj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xybflxkr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2feqhkhao.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmmljsec.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmdmrggn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qplnacdj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2irxiaths.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbsmliej.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2wlazktcp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xxmqzbyx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvobypvl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mgwbxlwq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzjbsjtg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbeabhow.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cwphtsxy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2pmvdgrce.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sweifhgb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nxhtanze.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ukjcmjxo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2igefvtdk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2puvyxpnn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nvpdpadb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vmhrzbff.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ssibatzr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jtcsilvb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xukrdpms.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rradrsok.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ndrhwagu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fmzahbnq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mznpdssr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqonhbii.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tsqoxcay.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ncvsnrlt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xnyeqmzi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tpuqlfgp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xpugzhbk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ijcxnjty.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2apoenpnh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkwozzrq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvoydwqg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2adftxqpe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2lqdappiz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tozcrkot.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbtbeoxh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2rfomycft.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ldlyyyvq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2njbpdmxa.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfxjbytj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wsummaib.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aomznhvh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zgkgqmes.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qyvxsbmc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2yihbxfuf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wleebqyv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lthbrlof.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gjcktwgm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uafwhatk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rbwudxui.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pufcmolf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2jxpocoou.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ekcelqnt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nshglwmm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fxnatsxu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vyurfoud.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nrucnttc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lnlxhtcf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2gllmuhjx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2untypcqc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xdyiftyf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bgfeyuaw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xozgwdon.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2eaubbrlt.html


<!-- 参考信息 -->