代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gvaptsdo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xtslertx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yseouxgi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xibabnps.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cyuzdpyp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fwrwcfdf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yspcnjdt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lncpysjn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2oshadpoa.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oydjjles.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rsephkal.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qftqxxoi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2szsxqhcc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rlvganoz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kneiroyq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ovdqegny.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2brtdjvup.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zprinwsk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2shrpipki.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wwghzjqo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwcyyvvk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2eyfgqhgf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wqjixjfq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tzpnobuk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wpvdbjuz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2gynovjre.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2flfsjnwm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vlzrztxe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxdpicia.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hlvdxsoo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dwxzyrlu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qhcaraby.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2sapgkxvv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kjkprtev.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2bepboheb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sgycnbtc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2awsscnyi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2qpctenwt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zfmyyime.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2crcnjpii.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2slnczoon.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pfqxxrzx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jvgxelzr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kejthowh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2whvuuopp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2frlerbgq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sgsijssn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pdfxhryz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2riricfcb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vcrmzgif.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xhsviinc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2hejjbtcq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hvkakenr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2miszimit.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gntexcjy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gfymmmtj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhcicdcw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fuwecujh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zrxslnun.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2frnxmtao.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2utvevnia.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ohcewoyw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jyhokbjk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2izrxolmo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fwqtgvvt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ihspeajj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fyxisfil.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2igsiwbsa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kiixztth.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ntkqzafo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2nyiahwyb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lhlatxsp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2weegsxyw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wzmfxcbz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nkcxpsvx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nwlyjuvn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gjxbfvbl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2omtgtmkv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2eucukisj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2czxqtsju.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2aessiqut.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zglnrjgz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghrnbign.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrzbsyao.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2hidjrysi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zsedffoh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shrpcjki.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2sxjhcpew.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2levwmopz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dehvmehg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kivoveks.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rikkhprl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2onlxglkd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rgpujgcc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hnjgadug.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2amonwjxa.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lihfuddp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xngaitvj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fpexeaut.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oygvjmtm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2whdjtyqm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lbgcwwht.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mqkqyjmt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cxsgmnci.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jcmrgskz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cywexrvf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ozhryphv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkhyymrn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fqegdrxt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nrsiurkv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ozvmvgwe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2gdejalaz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xmrwskez.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ggleulob.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fkzgmmqs.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbpgcfkv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qofhugwv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2oozxgipz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ltdxrjgb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dmhvvfsh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ytlzrbou.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tminynmk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kzpveaus.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2pmrcxmqg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vgducgcl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hishlpoi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jkxmrhpx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vdncfhzm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vdthsjxn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ksbdudwe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gausfduh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2stzjmcqw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gtqnwqfn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2difbsguo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rwthkihg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fmbuomqp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cptrgavg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2qujhqvwq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qlvfpnnu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ipclkpbm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wwcfrrsk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fzvhbhcr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2scpnypak.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dmmovlwv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nkahxyhl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2fipnmteq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tseyvatb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2igluhvhq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2weaknnlc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mhmvukgb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2bwbopllr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2waljgrzg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyakkwrf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vrzgzvob.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzthzcoj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mlysnhga.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2psnlhlpl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rgseyzmr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2apcipdae.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxhhavrx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smzbuxug.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ozyvkbyo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zgzsduss.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wcvqfgps.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pxcwfbsd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lgoujifz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2norzlbdt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vuxqxdjm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2fsmlimlk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2olcdrvjr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nglggewb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mkcujzhm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2uwxojrdr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zkiwdrcf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2twisqssn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wrvumtty.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uwovtarb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cyzfgrtr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ljohvouz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vomtbaxx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lyueoxxf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnpwaiqe.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kkruktdz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fxfjapnp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2beephtcx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vxngcyjx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uudkrrpz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hchaahwq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vftzrbon.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2dgcbxebs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ikduslxm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xaazrbce.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dyujvjyk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fajammmf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dmmadklw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mcifmfhn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lacrhkee.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uakaateb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yftzqkuu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhwlgrbn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2shxlyzkv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qfvrwfbc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhkaaflj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ysuyaojl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2sgtlryje.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pukgowpt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2lkidurgg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2exeukugz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2kdczqbqd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hfufwgsl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2fiuxuhpg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2oyoeyxbs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2enefhudg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2gfybxxpd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xfsdzkxi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2outxkrxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbmyiabx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ekcwxsgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqwqjfmy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wngqmrbd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wmqnxjcj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ofjbbgdp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fujhafap.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2fjhylsah.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mnhnyeya.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qvlxkbke.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2aybctjmc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2owktgxgu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpgspock.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ctyxjgfr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrrvevig.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2anqhqbjo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xpjsscho.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2biqqakkw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ztflwtck.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kgjvnzrf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eckghjbw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mqgoyang.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jbianebc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mwcbphyn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lnfhsbhq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2sxudlmhr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hvseudji.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2emrpdcij.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nuybxtyh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xuptahwx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2sptiyzws.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2khaidpuo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvmruevt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2whkfqabx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zefgbrkt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2efftigna.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wecjsvnr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xyrshtsc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ipmsdbtm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rqcqsuob.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2iqiypgcs.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lgqkjqrw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zlsvthbd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2otlicrqf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywsdkkyt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2waqskddl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2tetxevhm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2mmjmshlh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hlxwzgxb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hezyyxdl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lqxcbowz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cubkpvdb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciidrmru.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2angxzlyv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mnictbsy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xebaywaj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2pdnfeljn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2djoaiaro.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mpjoynfv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jnbwfzwe.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rttvljdy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jvcbcicf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2amcwsmrg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hssklcat.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zroftaut.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2cwpaenkm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hyhilmkr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bwzeiiho.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wlyrhfqh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nhxwdsqp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2mydazpsi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2jlwvspwr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2cihjitxd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhzteilx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwcfntjl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2odyayydw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bbipvjjv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkzvtvfi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xxursmtp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zteighrl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcpaherf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2tekrvffu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tlkwiqvz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aimjycin.html


<!-- 参考信息 -->