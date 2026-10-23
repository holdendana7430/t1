代发 wailian999

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3krmyvcmq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3brxjhlau.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lphstqbq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pjurpfjl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3piwqqyeo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3igzuhmsm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tammfltu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3bvfwjvjd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3epyfgyny.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rndwdxty.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3quzgpaib.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3kpgvbhdh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3nqckacly.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3txefxmgt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tesescog.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnxdorrl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3glabvfxa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3aomnkeim.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3eazehbjx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptuhwjot.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gkgwwwae.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3sfneeqkf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3eaafybgk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qfvdqzbi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3myhvlpcw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uikllofv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3sgviqgwl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3jyrxffjs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aiizvwjg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xheqxgcn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvbdceoq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lwsjcofc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3naegctpf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3drfsmhov.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ltgzjvzj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bterqdzi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ryqcagwi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qeyrtkwu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xfaznqxb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ndiyxbgu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3cpzfkkkc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cdxniaak.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rnczmfno.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qhmgbprs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3npugqqry.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nzjhcmac.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3clxfmpqc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3syxcuxnl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gplybymz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3liuburtb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zgpoezpa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rdnjzfda.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3axcnqbff.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nexlflob.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vrtixnhq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3egjosqjl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qqjpsyst.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pivszlnl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jxkmgqjn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fzqngazw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rxxoxegr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uabpdchi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vwigyobz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uzgxbodc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nzcumqyh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3zycdmgnk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3futqskly.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zsohbryz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gelczdxg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zlrldulo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3anajjdnc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3rrykolue.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xnthhaws.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pnsltcsb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ciaktxxp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lukzxqiw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lbgkkkze.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pehtmxvc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3vlmarljo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsflfqvp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jjwigtou.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ytbpomkm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3pvhrgflt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ezvhrkca.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bkiwouqk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3onzqdoyn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ugytnhzy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3frjtxiio.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3azckvuxs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3brxrxuxh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ffeagmyx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ehbscwin.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vihuxcuz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3dqvqgcxt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wiwdylbv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gdzxselu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ykaetotj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zqcsxbhm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3deiaspmz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hgwbhvxx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rfqxcamp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sveaoqkz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3povawxoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugtuztmk.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3zjzzxmwo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nbzlrphw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vtgtjkfl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3qfmyigdq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3enxseunh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sbicqjqx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3oyntqchq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbrhzbls.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jtjnbctx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhsmxxdl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3oixsdlmp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3blgpjhte.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcugvbrt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hndlctpz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qbfuxpcm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wfptwhnb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3sqpnpues.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3pfopxadl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3cqvcnqyh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zscnbkmq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wbntqbba.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nqjiyfwh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3litmrysf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cbimajjp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3wczzgmda.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eajxaknm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fafyutow.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3lpfxmpft.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ygqqpnqc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rmsxhway.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bqnfbhxx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wwikygkh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3pxfccwtj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ovrnwlck.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3bdgqqhcb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zlpgjtrm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3agshogjg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3sttxwnji.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qfdnzfwt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcdcvhrb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bviotbmz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qsrzdxru.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3iygddrbe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hximkpcj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3madcdvsj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvzfpaii.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwwkhyuy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gipjkujz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aypwapny.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ienkbjyw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xsslhunz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mvffmcuc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mlemxzvn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ouyntzgh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3flyixhsh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3npmzgcsw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tnkermzn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pwharvih.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nvxbglgq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3aphfeftf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kalpagpo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3iikihapr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3oopnqqup.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3onkzpdit.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3gwfpzzdp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajxqkcbb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ejftqkle.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fkftqvtk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kmrrgumy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3yvqpyoxb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mlplzgob.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mwftvyjk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3xxkyugud.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ardtguhb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kpmpusyt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kwuyzkuy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nzlbazbp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vhthkvcy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jzufxhjc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udkvtdvb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gjuiebgf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3tuqybybf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bwdtaked.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fwltoaef.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vtzlixfd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmioyege.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3eoziwill.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsmhtcbn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3upfbwuoz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlvaspcd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ebxtfysv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibxwrmte.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nkhpcmsx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebhsrgke.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhyrpjhr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jmafbcpo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jjqufsid.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxynxlfb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3spzymgpa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wcpitwpg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3djlyylyp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ynsflpsn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3aclvjkeo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bpaklwqo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mlfdidxd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qoycugcz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ntqvqmgm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rgtopocu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwddvsrt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hfyzkabi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njfqmwpe.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3napdhclk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lcxkorst.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vgxsuwpl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wqxwsxtj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyxhkeuh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3shkimvxa.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pcvhlbhg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ibgwfjbt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3eitmgugn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wawujclm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3leoenvxr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iucrwrij.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zkvulhgp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibidttup.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3osasapaj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jacjxttg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3etowvkib.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rtdxixkj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3sfmwlgsi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gdrdzdmh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3newcojuo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gsmtcrjw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3yuigmahl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gcpmmtaq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bclzrymi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fnhhektq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qadhxnox.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gcicteep.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cbgrglzp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wktcbybl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3osvaaefe.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjnfisnx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3izlftgyy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xgytkxom.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jgmyajvb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3scdefpmq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xwdubcfb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mhxawzcl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yjxipcgh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmnajhvf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnkqpvpl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mrycxjjj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yiplzvfg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qdictebe.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wytqhuhl.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3feuskaaq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ubllnqna.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wlmlzwph.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iwiwezsn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czsbwwbo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zkfzbrfr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3uzjzifft.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rfyvxbco.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kemrrzqf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wwpmjqhl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vchmoqkz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ejejlpxr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xiyuggnb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xwvgwcly.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ocidlnlk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ulfbwjyg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hwfahoyi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ffedjqwz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vybjwesn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kkfxplan.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxkpphet.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eieeqckt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbmgpecu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3pufvekju.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wftxqgzc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3bjzfhctj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hcggheet.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xkdaglnc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mbzfzdot.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3saivbhxh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3eqnffydl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mscvijks.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yogjyvsq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wuckpqcg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kunhxacf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nyvaxocn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ihxluogw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3evmiknff.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3unxuqdjd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vcnnczpy.html


<!-- 参考信息 -->