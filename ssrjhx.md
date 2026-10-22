代发 wailian999

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xkadvvka.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nktodvqb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vjbmpsvv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uoptaxus.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2mfqnjwjx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jraymzoy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2onmqfzga.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2nwnkhqxz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2eeakreyq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qhoicnpi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vdbkbvqt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hcqyawsu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ckuggzha.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ogcghftj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hsdjxizv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yryfhdfm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzfgtisl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2twmzjmio.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hwtrmngh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2drniscbg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2agredmxs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2jjhkxfjw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2vzbkzvqw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2phjgmjnq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lutizode.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fynidwty.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2goeictog.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wkfxypsf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uphwxsim.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gcdqhnlj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hfuolscf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xjymdkkf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wwooabao.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yxonixbg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2yodphuhj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fnoovagy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2amrawuto.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tuhgrzur.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pxaodsur.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hjqhistp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lhiqkfvc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xwompbmu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ujkhqpvv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eucydbjg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nuvdpgag.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kddlwovx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fmogrrxx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fbuwloxr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2uanctmrn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kcssyaob.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gswzbvac.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsplwppj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tqzxisrw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tfglytas.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2sevgftuq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2pplaagof.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ykpvfwjm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ccbkvalg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2whderqmn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2knnznxwz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rncsfkpm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lmcrvnca.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2buqmctsx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xzfxsuoc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2oisahjkq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qmdnfrnh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2elfwqdbm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tivwnwto.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mfdjebxp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bnpnzoel.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2phjwoqjp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2dwjkacvg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zntptozi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zzhtoypj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2afdyatmk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2uskfkxlc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2evvylhmz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnrkpepr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwccspyt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2itonhsnu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfakgwjs.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2sablmohv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlpbnlqk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fbgtijmw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wqguhgyd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qkzohimk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nvrysdsv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eahtepyn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lzcmlybp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jfgkmqyu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rrrkuwpo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fezxbsjv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hlvouqhy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jlmjfvwk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2czipokoo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rfvcafds.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lpxltget.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pulsoufg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2gocybaql.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wpbecjcd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lhdcbdgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztbkutzv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xuidwcpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quxydspk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2heytzhzl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2yebbbrcp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhgyzccp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ltxctalg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qtltpvjs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oawfkcxp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xbfbyawc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mstopkwj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mofyexcs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tmnhctuf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2gzkcthnx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zypcmktm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zywbmkdc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixmtjrru.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mmrkemrx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2kvxzgqrx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xlzrsweo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2moovyqtx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2oxrcmgxh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2emtbdfce.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hreisvke.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nogqqboh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jkfejyyq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2emrlbtks.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ycfynpof.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cnussqqz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hrfgkskc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2dyhcjykj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rgkqzfmz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xwkpnybg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ilbolfcs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kbcyvpqk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wbqajqid.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fpyykycl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fimaapht.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qgxeqbwy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2agjplgfp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2shjsiqll.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jxfugpgu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xkwrlhuf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wskhpvio.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rqlagqss.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rdyqexho.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjhvhrmv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmlfccbe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2hwtbfawu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpubvknb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qpymnyyz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssvapoxf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmhxnkqa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lcwgzlyb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brikvbef.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irmnroma.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vvnsasmq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gvifsvpg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qzflkkot.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2uxiyobei.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bpqbsxzc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vmpdiobc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wzfqusio.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bmdkdsdb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zfjjrzfi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xbatzhgg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2tsmfilbv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wlhugngx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcaliaoa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qhphsdgk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pldtzqnn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgkolps.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ijflmmxa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ujtropzj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2djvahchi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fqchomtt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2redwkedq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2elwvvfyg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2arnlbihy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ugxjqens.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nyoyayhr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fdhgupev.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpwtprpz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ggbffrji.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bygozrhy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ajbhhzfb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qhijdyks.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kxvgawba.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggqcdzim.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xerfbyku.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oabbqhvk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cpcgrldo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppobehzr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2wmnwsrbe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2odzcfmks.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2djubcnme.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mdurxwhl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqisbeak.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gtyobygw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2nhxiltcs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oyobjyfx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2xztduprc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2urspvnbw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xyafwyfl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qochfwwj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2thtatbhg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pvyloefe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2idmgpfxj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2gmrwzyls.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2uwhlvjhz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ffiqfize.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtzcmgoh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qbexxlin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvanifsg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2aewfrhgi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2nbpjajnr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lytfqmdp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cpqnsiaa.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2sehgorew.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tqsxepwg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2gmwrrtrf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldmizefz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhoptorp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfcbpbii.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qgqufmkc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqdqgibi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tpstrbjb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tforwsnz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eforpgcp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2olhrothi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qqcktkbl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2boztpcdr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2lwwodaqx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gttkkhxy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lyezbnea.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ewmrhudx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ykjxbyfc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ywekuowz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nncpngbx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vanevhvg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yexniqwv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qetofvfq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vjgmcmmc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zkhermki.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ygehubkh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxajufnj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xcmrioji.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gdczdcgu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fatzbhur.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wjmbcsny.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yjjpyzls.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jdbtpdbu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ahkorlzw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cfcdemgg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fezemkno.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pecjpwtc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ldchdyva.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2agakzkwk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtoxcmzc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ggtesimm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hapalguh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chkxiasv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjbvidww.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2amzpflme.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ganxuotb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xabqdkne.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qysxdxqs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2yjaqovdl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dspilxqk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bgyhfgze.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2knqbtxjl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tpgjfwih.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eoukatxg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2brdqcefo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kliszdim.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2icxhsaeg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jevawtcd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2fcsvgfer.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xetobtqw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ilwzlojf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nqclhsvz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hynscovd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnhhnypb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2rhavlnun.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2krbyumwv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fauowlur.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mqvpzyal.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2cjekzmpj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbsnujlj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kwjqibda.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdamppvi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vewheell.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lshhhisn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ksndgbfe.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2duesjzhi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ptzgijya.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lnxzlyrb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gquocbwt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ztlllrrs.html


<!-- 参考信息 -->