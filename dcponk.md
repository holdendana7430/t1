代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zmefzher.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pxgzxrzp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3krkwekoc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3cghjyuvo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3zarljcdi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3chydlljw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzumcsry.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrleyapd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fdlzatcu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3momiskka.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3vrkmivus.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qkjfcbcf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bfknkhiv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tgjavrdk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iwmblysq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3hxszryue.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufyuocyb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vjggpjzt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3taayddvf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3opchgqim.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3csrtebpd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3rkfultyx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgsyunlt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fzehbtrs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkyhpjpp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iaoqhhfh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3blvekcmm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3upnetgnd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrilmwcx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kmntzgul.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pdmmdxwk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3czrrmzhq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3azlxqufr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lptfosjg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gieawxfd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bxsscqvm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dgkbiwks.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mybbxlim.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wtfuhjya.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lfqksebe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uypcgdvn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ohldzpmt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ceeyprzv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3guaklsqo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rxuplrsx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3veekotyd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lsuyvtor.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3fpnujque.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3nfdhhvyf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3btdswwff.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jdpxevmw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nubbzqqj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jyhcaugv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gqkouwxu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rvzzpsxt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wvlspdtm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yfqeglzc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3djtflcmq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xmjfcjqh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yylnrnpt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3emrhtihi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bfgeszay.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ptjfmtim.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3brpllbgc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yoolsehw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tvnztrzi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3pfvttdta.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3zfvzgxjn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3upunliaz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lxvulswz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqowwout.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fcwxdisv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3iobymlfg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3deqowncp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bklgqvlo.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3etpraihq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3stzwfzbi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rzckcggn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fwblgrhj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3amacnvfc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nlbmkybc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hzktewko.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hlmrpssa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zdfzezax.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3lvffiupd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3grpvckqn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yslrhcko.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jnirjxyw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wwxjnzwl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ceqhqtkb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rshoxccj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xbstlgnj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3huaamkfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptwyisbf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3mmxbvmai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdrbvdsp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nlqjjmft.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3adzazqvz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jlmxonvi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ilbwlgio.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kbwvivgt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vitlzyuv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tlmovtxw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sazbixnc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uqsdbhyf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3aztrrwiw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3eqrujlaz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nhmpoaun.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gupxsexi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3phrtmoil.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bqqgwqku.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3umclgwyp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vglpkcau.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqgkylnf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vvxtlkuy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3lbirmqui.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mwcpfkmg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3doldslmd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cipvrvhb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yaxmxrti.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jmqaqobp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wxrmpgbu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3garyksoh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3csbazbdt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qphmlezh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3jeacajot.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iqudosvg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ekrkrbdf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dtavszsh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sdfwhbvd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3oaidfasv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3yatrmdmd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uiukgfey.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fabluqun.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dmjvhetk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3socfqciq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwfnirif.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aqmrzsgv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3lpxxielz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsheshrv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dgaiectw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ogsrfthw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3euouonuv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mwqzrhid.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwdfecjk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvqmhpmk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3szlolnpt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anyurecs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3slkpnhgv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wdrwdnwz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ixnybtgx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pknktges.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qqoddhgs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dforffef.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vwgwbadl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3phpzbepp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3buvsbxrf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vyhrderm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qffpppii.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xhztwybz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jxnniujy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvxcxozr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jiawkiqt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gmrzwzzi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jvkahldj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rovrysny.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3aivfdyoj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3khvemaio.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3oqdzvlhu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vltoeaeb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fwtscvbs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3temjeubv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vvurdgyd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ksgdmfui.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3uummvlow.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvijuqsi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gkfyesjw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hhxlmgdl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3muosulas.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dirsadwx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivzknszs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lebiwvvy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qlseokhk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbaequzu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pdmrxhzt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djbyooeg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3zywythwt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yruscrls.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3idvdwmzb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sptnkktk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjtdikws.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrcmyztx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ptvdwido.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdkmwqwj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xxzarbed.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3oeyakchh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3nrsjyccg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3pzhsaoxc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3aljcfelx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3eihcagmq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3njkrpmwd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3oihnwbgo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zvzeagai.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rekdgaah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtwqywhl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3zujlyprt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdrbmqix.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bkjolvlj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3kzxojkvk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3shmlejnw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uujznutd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qciruqfr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wbwnhfyb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wxetjtoe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tcxkpewc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjkgltpz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cixxakrg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3lxweudww.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kduvpzmq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhirxvxk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkyiehdc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sicnpjcc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3soqxlpdq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wywakpxu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3guvstuvs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ddpwbxhl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wtbrddig.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sanvuyvh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eujwziit.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3txrguqfy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3lkzwyfdl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3dgortirw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gciqkdvi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3czcwjqtf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3axaymqzk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3viedjtfb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3euanrofq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eyhuaacj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sjhyittt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuatkuth.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vakvrsxp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3isfvhwrs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rfwpifxd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3iwmcjefj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3hzkjaasj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nppqjphi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ecebecbp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qurmzjxh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ykoabkbw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kmjspihq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3verribqz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtjzfnup.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kvscqaok.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hyksxjpj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvgcqhpz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wszcnomj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3coznzcql.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xnimqxgy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bbwdmsmw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mjzbmdsd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uaghhkoy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xldqzjvz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3nyyzlthk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kpcreeoq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ycrpzlrb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hrffxgur.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lmfqxxdg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kaabqasw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ncbxnasv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lvugcbay.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3igepxfbs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dsmdpnkn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3llgwpbwr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3pxjoweqf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlfurkts.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iitjetcn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jwntbwxi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3yimgoism.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eafqdobv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3byueaqej.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3fyzxnnuh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3elyrldac.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wpwmzxxx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zpomubxv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbyqrycy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hxbzupyv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kyolhjlj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mzcpxgex.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3tqyxouer.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3duzpjcxb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pavdvkmo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ahouqsdn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3avkuijim.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dqcnggap.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gbennnos.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3awshajxh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3qsccstlp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3abynencc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3potpkalg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3palyqypf.html


<!-- 参考信息 -->