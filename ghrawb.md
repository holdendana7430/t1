代发 wailian999

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3indymvrl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mmdkmatd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jbydryxv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jilhgqut.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3bdkrdwmj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pugwwsfp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3reuwzxuh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dospblur.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ldnerszj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3frqnszez.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cyscjylr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cjxsywxy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gumuwkqd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3efjagdej.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kcakqmoj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jbxzluog.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3owhpvhfv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3zwczjwpo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xiraurij.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybyvlxpe.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3swtflqde.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ozqnssre.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ihwohzui.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3syivazxc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3wocrgplg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dwkjhhwa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3duyisykl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tgylxrdz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rmonuqsa.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bbvwijfn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3suzjnhfp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mmudjcdi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fdqvtkkm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3dnftsjcg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hxylrolp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ntsbdwtx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3turjpyuw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjfsekor.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ygcaqncg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kjhjrlkg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mhdelorw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zcoduhaa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dyvceieu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ajneeyhi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pkfordxf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nmgqldke.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jncqromd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3yyuxkugo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3nnwvcwix.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tmurivwk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jbsqjiob.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3thdffxhn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3njpnmazh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3oiylscsu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3avzlsajl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3nvcqouzv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ltffeuuj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3oyzenlcz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mrxsepct.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3houbaddp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gxdswgvw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3egtkusuz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gkuyvdgs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3omuqqqlh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jbzkdnro.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mhdarebw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jnnikaya.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lnjwfbgv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zsvsayma.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jrrbtbbu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qbvswyvj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rpveeqpw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3phhwiqwf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3swxeaiyr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vvipvbyx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qtlgxgnn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3iarfkcex.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypyalrqe.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qggwhquq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wwpitmng.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fszppnti.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3gjnitxhx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3thggandl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xubedxkg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mmnwvalj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gpyuwfkf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3byspbfjo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tdxsujzi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3umxcvwzw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vyypafra.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3efrnyprn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yhdictta.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ddhyozqk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhzqnjc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fdumgafm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dgertpsx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3barugqqu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uenwnftq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3lcqlagsr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tiufqguf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qsudqxno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcbwmpag.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gmvxrgdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpocmvdx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3prxsazks.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wfxucnyz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mmdaksqx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vearssxu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tiovdosf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tkymjxjc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3yhcwmbau.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrtjkeqf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yvblhiue.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3cgnikwil.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qhutlzzk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3swopdtce.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltufngks.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3foazxsro.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3irbhmeul.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qvndcxzj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3diwueczc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3eaivpqxe.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3oxcevsib.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wyeixkmk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rzfovnke.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3topmchoi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3exmbtoap.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3oefgevla.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fhyhbvud.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3neizkluj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cicnrjyb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkkiegni.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sdqveqqs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ppmpoeap.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tyvrgmvs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zmmupnlr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3mwhcmahm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qlzkeacq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3hwuvzymu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xndwfhkc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zwchcjbt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hkjrnxnj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bpnmejrt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uedgrkbx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3soxnoypt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bawnfsjh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3roirzxtk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhhhvpxc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zuqcytea.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fzrpgduu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sszcojcw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eusxwbhh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rnflewqk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3enbmbqwe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qildgaun.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzixniks.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3glufqpib.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lfplorgi.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jsawqiii.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ylxrzswt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mnbveifl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tjgdzrky.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nmqailpw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3dvkmioaj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qzvfdoay.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fpejkhon.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qrznfejw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3caigzthg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bjelnzei.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3nlajszgs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rmznrcje.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lsdlmpdg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dubuooxr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3vmhndaly.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xvxytegh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pyqosqmx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3yymiyjur.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zxrmsihj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pzqxvybd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tcprrxuf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yfzrvokv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xwhmgkul.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3riqzvffr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhkqvokd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3qswyftvm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3spgtabar.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eeyttcnj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uograozo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ufsaupsz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3beozfkel.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3slncbccm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfngxscc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqewmqej.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zdmovimd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ygpntbzb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjtcnikz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ecccnonx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfzceaef.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3obccxiwy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pqlgxrfi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3trmzwync.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vodzgcqu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3entvlznq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ackjbfyo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3yxojnhfa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3yrdpvcog.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ixjxfpii.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cpdcaeph.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rhdutkfd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vnkezpvx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mdfzimrr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3dnvmnwoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vycpkedy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3yjihdexf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dutnwhxg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kowjniap.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vwqxvpvk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulbnfyiy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpoazwlc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tummkulo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhvfbvst.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yspttqzs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ssnvmilv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ruptfdcj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3fognqppf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3uujqbdqa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bxuncamj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxteppct.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jobwzizk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3aytledps.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3woekvxqy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aurazedt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shucvohf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hdwpxfbn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ewqztteq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dsmimlwg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ipostpql.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3uadadmue.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jcwrqwhd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qogmxrhx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vxestmfj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3sdnnpakj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jxhcdxfd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hwsvezhu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wqfwvsrq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3damvrtwg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lumnnxov.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcivsllx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3etvraecq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mdgocjru.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3akpagdjk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mahxtevk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3wjhbfalm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vjolaglw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ietrmpqs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hxvzmnyd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3whpzowyl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3naaisfsk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cruamowo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3tptsbjue.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jekcudxl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jqxffgaq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvxmantr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lovewbkg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uyqnwuul.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgqocluh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ztjustvb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3muejlkvc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3rkzrktli.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xjteoflf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hfjloolf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vzcqdxad.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pykwrfem.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gwiqurzl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mnahyump.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jaiobpfi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3chqaeqhe.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bqzxlndr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xvmhqomo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3slbldxcp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pnmxhrjz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3doubivot.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kybrqgfy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3exalsyrx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zaxfdbkf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3chakgcmh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dexmqptv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gzpsdojt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ighrmrcd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3iynfhjte.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gefmicur.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jprfmhav.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzcabioe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qrnylvfe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ixxeauax.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezxtvwgw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3mzooyblo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3wiastrib.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mgzjrfuy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hscuilbv.html


<!-- 参考信息 -->