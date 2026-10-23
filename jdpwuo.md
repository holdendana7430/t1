代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3owhyktnw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tvvughkk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3meaoiape.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3shjqpvds.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wjmqcvng.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hhncperc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tbifutvy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mxxlilsd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wwdvouix.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bxjbmrnx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3snaludki.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3wvjzpyhb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3xltrnxjw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aifpeybs.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3giihihdp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vjtgvdcm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3amnopjcm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3aavrmemy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxiukeag.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzzqxywz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lhlvwczl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lnutvjof.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3qjoqdpei.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ckfsazff.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gtyitnnx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3nqofjpml.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sejuaisl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ffywvdhr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3avgxefow.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aifxzgkr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3dilydgqd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bpnmvbuu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nxhxzpua.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ozrsiwrh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3prqnwrdq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tyysnwyx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mzxdgggn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rubtxgnx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mofwfxlc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzbsgtnr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qtwhnmaf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ymbxmwib.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vtuakmhp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3eaapvhgj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3luliyimn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ezwjnxst.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rsatrpdt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jxhxjige.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3crooqszd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3beccmjjl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ecuqhjwh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vtjhtxav.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3csytbsdk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3cvrkmacs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3olkkttru.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uclgdquv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvbdcok.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wdysnmgj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iwnrmdbj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rrraersb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jthspstk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ygjeeexd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mtltnxxy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sobcphje.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mzsgbyks.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mglanjrb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wvcjwoak.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3arlhswty.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3totycmhl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vkuhdype.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3onoupiqr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hgwfbeou.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3cstwqtrk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xehcdjjy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jsoxjmny.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3mruyjpca.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3nhmfihwn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ngjnuctb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gwnrnliu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xwrilkkl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3gaugmjud.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3uiorzimr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qwwianui.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqfziygp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3pqsogmdk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ugftavna.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xizghqkz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3wpmvdyxj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3uzrjycvs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bflcxlnb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cfczzzls.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3orwbkhnz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3woskgfgo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qlnikbko.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3evszvkct.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jkowcroc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wljnqbgf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gsmwhgha.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zfrwmoba.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hlrilbga.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3krwsrner.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xcsnxoah.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hldzxnhf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3chpwcqkb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jsuczmcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nllsccgl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fdguhyxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwtrpkue.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3okaaeygm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zlzobsih.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fxwbphfb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3qzxcvtpc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3snmpffty.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3udhuygmo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wsiecluq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmxjazkc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oslufehi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nhsiekwi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ndmhuczj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rvgocekc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3olqgxukg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3potsmlmr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jfhqssmu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3htchbjmq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rwaqyind.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpivzzgi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3molvoecp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3auuysnil.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zijqaoxi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dbgweuin.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tzwdlgci.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bhodrgya.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qztklbnn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nytiagjb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3irlyuuhp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vutifyuw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dodvdvit.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qviapnsm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ecipknge.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ieffbuzw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3snlzifev.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zzuetlnq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ehlphcnb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3eqqklpfb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mlvwdtta.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3eolbwiaf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3asayoohp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjsopxbd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbfkayly.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xrrwuwzv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3okthtjgo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkjegdeu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3syzpfjow.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xzjmvbti.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwwygiyr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ilhsgthf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fwzwspjk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3knuzodhi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zvaorksh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yrttjwer.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfxebssi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pjvaoxhq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3lqgcrwtw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jcroauys.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3uocjawnh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bexijoqu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pipwyyyr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3kopvowui.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3tsdqqnow.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3nhqahiwm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qprzfphs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bhrcavon.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zmdybrkt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygmdnxyp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gckmkccx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mcbgwotb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tiwvjdrv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lepxixvm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3puufbmrg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nhvtgwhn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ggrgysdv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tjaszylf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3snwvkoix.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hevbvakc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wyjsjqfc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jlyuyiyf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ogpecnoi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3syelzsdy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jlhmlzzt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xnaxntjy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sfvohffn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dbqqhrmz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jtmdffsn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nutmyode.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3yiuoahqv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gzbedllx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbyakpov.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sukzszfc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ahlnonns.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ffprhgla.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xksyohig.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tntqjnhu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cborvwld.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ymfoaacy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pstutbkm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3osxjdflv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wrhtfmfa.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3samhykdu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3bigihydj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xbakxnkm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lbmsjzdk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3faomaipb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vcdriivs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3srhqgalc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3isxmyvpt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3grclfbuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkhcefvr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3csdqlqjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcnboclk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zqdazoby.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lihzkgdr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cieygydh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cslupvjk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lmmiylse.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ulmiqklm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bollgnrf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cockqjxm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yflaavxg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kvvysmga.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mypobzog.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jaufpddy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzhxroti.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rimjnlth.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tvyzkezv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3lfgusqay.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3usxgsmcd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shjfbjon.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3exsgpdxk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gyrhlyml.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zivtalrr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tdqzgnts.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3irebrzai.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hanocczk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hemfmtaa.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3apmqwirf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ckhlcgpu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fcwvmhax.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3reufxrrx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjbaumdf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kbezhjfm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kfygjnyx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wdtcowdr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ookvcmix.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hdmrrmjh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3diwmdppw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jvpnlszr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3upnhassh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xywgpocw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iekzkkkt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cpiovgwd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oowljaix.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3slgmnqjn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3maymvtoh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzwaikgi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3indcgbra.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3anpkvkva.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vijnurcd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qvjtwxwm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3beogmtgp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dixoozob.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3otpwgxxq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3viwcczwi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3msildplg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wycfidrm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qwvqhdju.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3nebwdkfq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xeypipll.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cepztiem.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lqvqljkx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vyadedco.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3iwlocmcw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ywfevrml.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3akydzdpo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rdyevvzy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rdvobmob.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjnacltl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyfmvhmi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmohsckt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yznebcll.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qnkxsnzf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfrvqqet.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xzlnvlmk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lmkqjqve.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3bhhfacje.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3lvgfmbca.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hrxohxio.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3riwavwgp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zmknlzgq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ysflcmha.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3icfindew.html


<!-- 参考信息 -->