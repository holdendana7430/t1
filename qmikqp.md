代发 wailian999

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3frgpuctq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zvpbxquc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3elazhwoi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3duodihsq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3cnnizsqy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rubvtscb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nhzxgpic.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gqajvxsi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vdvprsqe.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mgvskawm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gsphyqhp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3eysqquqf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qqmcmelk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3wetlcuvg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nsnlcpdl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksiksikn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jmldrevp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3eaxviqmw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3kcqaoxgo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zbtahktg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3bfagelfq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gqdbhjwz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ajlwetfu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3djpqgeyo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shnyzuhp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dtcevgtw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gvbtnhtc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3rjyrcfgs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tuapvrnp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vjywcwba.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sduogetp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yejenktz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3cnuwawhi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xifpnmql.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3fopqopfj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rifhxdtz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hayyerik.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vfvibbgq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lkagyshh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3uonbeqza.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3tkvzanwg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3labflgdv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pgahgjti.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rrslxxor.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ovbtapjo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ynhxeyuc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hzvfxffl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ixnfajdr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3sdyisqfi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hcoaxenx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vtrwmtht.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bjepfclk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ygfwsspy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3agixrhnn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ttwwisku.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ucvrzzpm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rkmhksyr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3wibaxpbd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nvgneqac.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aduudegl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xzcvrqbv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3udlxexlp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ddowkovc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3libartbj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yytfoyxi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ulhldprm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3pxlktpyb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qtpittff.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3enyexwfs.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nvwrcbgl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3czbijawi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3usfjkqbg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3nywyfrwk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3doqubefx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vrhucydm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3vydqupbb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nlxvadvd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwrwsbfj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fkedhyxj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnjnwamo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lujfgmwr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3tkpcifoo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usvbpbms.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3excxxfbe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3tubipusz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dbufxkco.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yhcjcrdq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dcwpuylo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gizwlkpy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mvtiwjjm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lytsykkx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3epbtojgk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ixhgntlc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jipqcvwt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jkkzdkqj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lrngfsxa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3acfslwcw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fzlxuuxo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mqbfdqwd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sprrhagm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lgxfzqyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpgdsswh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3xzdwpzaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnqxpuum.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjjobdxk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3egglwqbs.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lfaezxhe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3myqcspgv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pgzjazwt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rllyofcp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3hrgzsmhq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3seqnsvzl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qaddjnpd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qrzoiofv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ustofqbn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rggbxzvk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mgjvfvxd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhvshvbw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zaypgtoo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3iditxrqy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3uugdwypo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vnydjakf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xibfhpom.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aiaopalu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3upsnzopj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jhyyipmo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rydrfnby.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3nwztfjka.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dmcopmsl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cwctqpnh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dszessbx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3bsvqevyq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iedujiyi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3cmadelqy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vqeqwwby.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vrvyptco.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3spipmbcj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tkigckma.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gsfmgnjf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3islhctdr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oypowlum.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xflaudrr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fwrdhwkz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbleuaqt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ocorcmho.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cmqhqgom.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ekctvwqv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flkxwqak.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpzwmiks.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ukitiwtt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tmqdpqei.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ffapijbe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtngukwo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wbvayqhx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3czyorvuy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwbgpnyj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3clslahyk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3humutcja.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bwxbpiyo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lhpcsrau.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ukqikzfa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sxsszoxc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vtcifwus.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lykeczau.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3aeirdrza.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mdnhjjbj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3volibxfj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ezccesco.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rgzpyncq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yvrpwhoe.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3winoyxeb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3psbqugtt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sntnsjvp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nyevulah.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3uffzshmm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ntoxryom.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rfeovrox.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3acsixsvq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ijkpmfjf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wvimtgbb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jyyikzpz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vyorrhvj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qowasclr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yzumrpzc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3nrzqrmyn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3cptisxrf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqeyfcrp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3whoeancv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3drvzvnea.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqqkremu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3usqdwpwk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfzygmrh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ndncqtxn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncbzqwei.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fjptpwrx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hefkdbzz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xqvdrpay.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cxyznqyr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vmoyvpwv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yeyevulx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3eaoneseg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ervfaxkn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jktjqwtk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xofzgkil.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3zhcknkid.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ihzmxxpk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xwrtkdbm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pajymkzs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3macpxlfo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3meturazk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fzwjkynt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rctyepnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vscqafwl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ysyvxvll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqxinsuf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kmzzlmnc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ucrjdcvj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xoexksvp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3btjjhvxp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaurqvua.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3bioxzuya.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3jnhuoqcv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hunfzmxu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kokjdvkc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zokluolj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3dlpppbjz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3pxxuhlib.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhnuojvg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jvjgvqew.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mzqxgwnh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vqcmqvtz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3osltesyk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fgrkrppk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fqqqrbbo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3iiuigbgx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tmhsognk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rkoqnzla.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wywbngzv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qxqxjuid.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3drhgkgai.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zeutkplr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hzablkps.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hzysrkxx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mpnbksfe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pyzjgldt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3swvhzmdb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tnlxjhxh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqahakcv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kmemyhit.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3soqxtnlu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ldrfukjt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ecqxwxbb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wlqmznrf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qsczpmwr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulpdctty.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ypbnwdcm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhfggkdp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3viaframe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqswuwgs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ekthgzkn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ubhmvjon.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3achhcgrl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iyikmgey.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3duhahrrh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdnzfnkf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lnriejdv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3pfrcpfyv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hatpipsz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3whuztrxs.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3sgoebayl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vagakyzl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3njitrwqn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ksdmeaoc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kjyacqql.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3scdbnplf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3alalfqrf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kzgxpnae.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ezsiybfl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3pctoexpl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kezjgzmk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zynhksor.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukkfrtby.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3iunmzfyf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3neyexmbj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qbfzwbsc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3albthukp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qffcfszg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3dlhwagel.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zqyvqeav.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxaflnji.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rswysxqe.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnmucvps.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3yykguunm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3iyzzfgoq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ivdrhnkf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dkgzgbln.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jsfkpllp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3uhxlshwu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zqpqsngm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mlxypsos.html


<!-- 参考信息 -->