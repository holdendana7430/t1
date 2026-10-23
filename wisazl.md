代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3guhpwwds.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3keskoadu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gfociqob.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xjctkzgc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zmjojjhe.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zeqwjrpc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pgtekztq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ngegbqei.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ntiqlgsd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3wobvpodx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwkpvcku.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3grviwdiz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yqzyjoqd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3znzcyxhk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mcvytebc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fkshtljo.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qmllsvbd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3fovcmifm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3exuydwsv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3skrxaova.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3edrbueai.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ljkqkqnc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tijidcud.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3dtezrehh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3usezsfmn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tcfytpac.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3pvyjkqeh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3isdolihe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tojftgup.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xpvxtmpi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hjczdqmq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzszlcdl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uosvrqal.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jzgxndsq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cjeatsve.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ecvnbvcj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3fuabjvur.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xfnebyjd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lyhhfhji.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xfpggyfy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3pazktmho.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ehpwaliq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3anizlfbf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jxhjlywj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3camglmbc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ikxfkblg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3itggrbus.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tomohncy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzimokau.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3cobszizu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ujdcnzxc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dkfvrhui.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3msydwxjz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3scowuvvw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jqqtaqfp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kiedcinv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uheyytyl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vypjztpf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lagqmdnx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fmspzemv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mzxcbnoi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zbbikwge.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tfkqqzov.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tsbdxahb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hntlruzv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wyvrtsrt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mrjexkhm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3sjnkarlr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3lcgpyinw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3jtgsmlzc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ysuqinim.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3kndsfdoe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3pusyksac.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3mwfyxedq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3uidtadmf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdinuwhm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tofwpbup.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3mrwsofkg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpeofjbk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3bwmututf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3tnwhdcye.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tumdcdzd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rcztmlew.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hvaphosg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ulumvnvo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ychgwusa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jqpmtwvq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3obzjsmdq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ryxlqotp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bksacflq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3skhoiirk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ogcvycql.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3emfapspz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xpznregw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ycqqvnvx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3flmfegzb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3saqwjazw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arprctvt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fbnvriqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibrrddci.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jzymsqkx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3oevmimub.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tosaglac.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cqnmtdma.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ouswyvvc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bveesrjd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3naxihuuk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsccifvq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrfiiiuj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3swjbnwqt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3gorbywwz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xvoglffl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcyzyxmu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vjuvvlnu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vwooobhm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qiddlajp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cgyuqrwm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3evunhtmg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ftxwoizj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uztgzhvj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bvgspesv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xwxxtoob.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xwekfgbz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3muovaqdq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jbipkofa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3urusnyfr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uijkrubi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ajrjzlbx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jodttkrq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ewgzfxbg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3autpptvq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kckagfqi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3wadprqlq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rqucfvwc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cyjmuqrb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tiazbwop.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3puqncoqi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ehiwrwgq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tqfkfsxt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bacnhhpc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nsdoydng.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xrsczudf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3rmecbkjw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dglcpqux.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oophifjg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3izqzxnpw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmusqnjy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xqfftyxm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wrqzoluj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ndptwnyd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dcdrxrmg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdakufva.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3imjxsqvj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mkcoyovb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xyurmddw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xdfsyuxw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yxgxxjnl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pjtvimbm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jsakodiz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ecqygsbr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3evmfsztk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3uzzouyxs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3dnwujqbg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lxxihirn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jvjbkbte.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqtkqkhs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3eeqkygms.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jcbaefzp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lhoifsnr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dbcwrssf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yizvdece.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3azwlbbwr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3aqjmdmle.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocvbglxs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cencnoup.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nqnvpioe.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yikrjucb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hfctpnjo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3stayyscg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aegtejjt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3whvfzpmv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3fqmczyfp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cmgjiasj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ibfhyrkf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqyauqot.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpoljhvm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3yehsvnrv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cstxgkaw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ghacllkk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hklecnwq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbdqewnf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixtsmnle.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qlqkfbol.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vqpnpsfb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwexjhwp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pufgegpn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3licezive.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3atukjdmr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xtumifgj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qzrlqwyc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3udhgdrbr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jwucnfvp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rzjmamlm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jwebkqad.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nckpjnoq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3bnicnohm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bagftgyj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3eyjknlea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikguvmyo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3bvbmgynk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvatuehb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pkxotlwn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3fyoravrb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xambvveb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yhwqwwle.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifieixfe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3udeyyrbj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jlqnhxey.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qdbjfalr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ueviaaah.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3puljoblr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mmeildgh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmoncxhz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iedcgfxy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gzedpmtz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuwqwycr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cuoupbml.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xsqwckjd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qemmfmzp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fqnpanfx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tfymjkqv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ejymddig.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zdfsxoqt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rfodbwuo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3sugjisxr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fgfnxczt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sccxuppd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3tmautnow.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rsvxgikn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dqgaporf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwjntlby.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zusflgcx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lpxzpbvv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iadlxgmu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jonajllo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pweyadib.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xxveqkim.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ufpxlgph.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3txsuytwv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlxdoexa.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqkwlhbt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rdzsrdmn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bdanxbch.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3pejvhnam.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tpfqpjlx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvkqyggy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xmhhenvt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wrbctjmi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3otzcvcfp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gymcdvxj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3snjugirt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3koaoodpx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jmkfqcab.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3czodwhzh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ccfkfgub.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ptrhibyn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3yqbghpqe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hbuuedim.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hpruawxw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xaqjnpgo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fmilveuu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3natfvcns.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3mvqajmds.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ndxpxdfn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yhpfpvoy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3uuhngieh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xaglwkpn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ysupehzn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3juoxthku.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwfpgnqm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3xfgfffag.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uewmljac.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oomymaje.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zzmxdbpk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3aigogwpb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvxrmgns.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jruikuow.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rqccrend.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lrgwicgx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3oyzdbxgq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3nsgwaxzz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tbcwnlzh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fuvmpufq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3uckawuqq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3djlimwrn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zhjluptz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lwcnpgjp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3vbbduuem.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3jtyizkac.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bheyjfsz.html


<!-- 参考信息 -->