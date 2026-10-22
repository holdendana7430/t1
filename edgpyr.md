代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2weonrsmt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jfrwzlnw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jpphxqub.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hgjmxeiu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ynrnlbvv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sobwzmbj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xjzusqwa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rcghayhh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sxwupbak.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mybkmrfl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2izdtznqk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2greozlub.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2lsbwekxs.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2imshvkai.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xdrtygbt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2eirnwkfr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kmrturnr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nyxunnoo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2lzkhrwvx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lgsvhgtl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xirozzhc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzdblklm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqhryegf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zuzwirbr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sixngexg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rtgivqes.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rmhpwuif.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lppglxei.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zbhznmpi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2zbuhavvo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ihuttjer.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vkvewnpb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2imivalgy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2eozjsavg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2oarwwuqd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bqhloojd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xsfzjxna.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2rqvusoum.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zvdgayxr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oknslwwd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bnxdkdzc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xlkwgepi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2savakppp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bqiachgk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ggebshje.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tzxpnlmi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ovxyuleq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ctthalkk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2asfwgjzf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kldfejrq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xsrjaadv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wwtniftm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2vkmrpbdl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2hmxrgrbu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ofaeexxd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2lrwgdugw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xjgebehj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zfwyxtsa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2axlsuowg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sydrmspq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tdldzwit.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2enltltds.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gcpqyfca.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2owywkhep.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ofgwhjqy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2aqckqtjz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2raurbpws.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iefkvrkn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ibsqvnde.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hxnkqgjg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hecvojzu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2sldgowut.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dclgnjxz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2piiizgrb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hejtifhl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2evtbfgck.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mrmekohx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uhehbezb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2eeugvmne.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qwsrlscq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2udcinpza.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2sonkyswn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2phwmoqsa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kmavqqry.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ixunjpce.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufqjrskc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jahtvitp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbapvmpw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrjyunbt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2tnzhsteo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbwczofb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zkjwzlho.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2uptbmbyy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ksaysbag.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2shuqidws.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2olbuewgm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jctrdhnz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qwwikzgv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lizxqqhk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2axkyvzlk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fnmxncjw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2juvwzcvp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2enswgvbu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jvnkhdtr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zdsadfsp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jzsqegly.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ufyvjkbn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2odtkuygx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vdwkejyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvvckrwg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ztazvujf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crfspisr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2soepbxru.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xvihcjbc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2osqchbqf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xtrzaegq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ejcudvxa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bowtnntd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tdvbilbj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2epjgpunq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sqysvuod.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2omozosew.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2arsgnbqq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijzgxove.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2goywtkxl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yemawrsa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2arvlbhbw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jdrljdhr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xczyawpf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kocqurvp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2lafmbsfy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xaprvnea.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2presdlcu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mhxnkfgy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ffmlbolj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qgtbycdn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xqtsriyq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lkljvznm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fnlysrhq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pxsmuerh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zdtczjqj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2cwzklyos.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xgpygxfw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rviziriq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mzsowpbk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2trcbsuun.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mwjnzhdn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wpwgyisx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ttbxwvlg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2yuldlxnj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2owlwrjwd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgucxabk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zyrxiftq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ehakoffv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zbymnrbz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efiyiool.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eohqvres.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tggrhfdk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxrsvutz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cilwlsnr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ideymkzk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldouaeci.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2awigefer.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dundswga.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yxpgjnxc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ijuwxvcm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wxzjugvu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gohltpyy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fsfocbnp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2prkhqosl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xiptclwp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fmoqlibv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jmtfgmpz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2oxffuybb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vcxnlhmi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2abggwvtr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2cjeclzyx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdubtuqs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jlondlee.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sijbagsi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vubgllzr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zrhffjkn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2abdbodjk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cnvesgqp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nhlowuhq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbwowazn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eoxcania.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2egvigzzi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nxixypoc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kfvxelqq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nohoxeep.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2frmsjsup.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lddilbnr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jxylebru.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2trqoqqoh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2psfybdfm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mslugjcz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpnpcrvo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pmslkpsy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xpuvhyip.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2epdghsrv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcahudwg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2zubwoxsl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lopkicvt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uljllzrl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhshvroy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hytpwrqn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wqzgtkvr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2frhaqntq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plrtryvd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ooiaexeq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mkhlpgym.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2syqtwaui.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lzimczvw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xfztulzm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mgiqlyni.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ceuwyvof.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jmdhyqir.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gdpdumjb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ujidyfzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2deocklzc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2fbezardi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pljxwfvo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2pblzcmoj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2paheesic.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dxeoojif.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjmvsqbu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqzqcoaw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjxqwjiv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ylfrjrez.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cctscezw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojgxhoys.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2dtzlgzvt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2brpzqbqv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykebndby.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obioukvm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ynctlqmj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nejsnmcn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2okruergj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2iazvlhry.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrqegcih.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2satrvzqe.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vkfayrai.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qzwllfov.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ltbljkrx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2spbhtixc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2flmirijn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2asoodhmw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fgxubaxu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bmfajbze.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kbniseyq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ndurnufc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lufhbjim.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbeumylh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cochjyjm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qnglvtgq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fhnakuio.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2simiyavh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tiygildj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vppsonpj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rwerghuk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vkevwnfg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zznktxkp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2frvcymmh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ffwfxapp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2iyvspshs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zdcobihu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvplpwyf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2yfrzblcz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2mpboqwcj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xbzwzlwb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvfqjksn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jwvfdpns.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wuczpzmy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2thwtwfad.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ubyavkto.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ygqgvrar.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kiwaxdfa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2euselodg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yryprqwe.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vzwdqnzu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iiuyoivn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uichsndz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2psqajknq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ffxavdfc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aitsqvhy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bbgsneyz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cmzzfwhy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kfqppwbz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmvqblne.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2goyugyzp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vjkkmevp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hpizovfy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gpxakiuo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnyossqu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rdqztzbb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bkrdncqr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2omlbgkpt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2belsljrw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzllronr.html


<!-- 参考信息 -->