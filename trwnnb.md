代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wpfvdwfe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vopkotnh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3jjzdziiw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rzgfemjm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ogwyhmdr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3rvkvgmag.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tjymaglt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uqzjdjrx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ajqihqlj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sxlqsmqu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3btpgkldk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xehntwdv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3yxeeasil.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ifruhzbu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3lltlsgfn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3srftygid.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3yijnqxrj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ynjvsmci.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3cleljwef.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3gvwwjskh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sfrpimey.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3yptrsvdh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtrafrot.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fkiebezs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vhljcsyd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3vszfmpjn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qmjclhxa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3zkzlrled.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dnosufsi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3temxnodz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cgjvddza.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3alegiowz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rlxrfqmk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ffffckxg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ingyxgbd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jgmocsha.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3erviaojt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ckaomyfv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nbivzmbo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3zsiddxtd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tlcowkuj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3sasdolkw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yoeplkst.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jflkwjnm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjcbcpmb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rhwryjcj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pcutxyhr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3sdhuqaer.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3posxscju.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fyhbkkrd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ftotkria.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hhprjkoh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xetymjbf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gukueays.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mmfrgiwf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qpwrytpl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cpktxijn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3slydiwvh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ucamllvk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gywddxau.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yyypfzsz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yyaehepr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3exutqotk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lqtumwcy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3yqhwjvno.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nwlnypal.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3eiabuqjo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3uruyhbhh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3mrbneper.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlletsje.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3rahfywzw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nuwmffok.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3umausneh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3opmqgqon.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwzjbniy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fsoyaidd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3hrzwzhpm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lakqoskx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hiyoglmu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cqilfpsw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ylxjloft.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ovmzzcjd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jmpccwak.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rbazlgqm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fchmhpev.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jpaifezo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3swxtbtjv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xlkgxoiq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tojyodtc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gbczyxmv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hhmotwde.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3riqukmgw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3unjlifya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrjiikut.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ijhepuhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bljkgysr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ugbidyhl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xqobeowf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ypktbssc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hyvaeoid.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gorgkxkl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mnfenbjd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ljemiygd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yevmzbil.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3naujwmma.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqxieyvy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3kxvrbabd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3wbldgsug.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrhqfumo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dizurtxy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3shdpynxm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qufrpzap.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zpxbymsq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajvxfale.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3rumfvpcl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3btstsawx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hbflyuzc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kzouilqy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eoafetjj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3pzuswhol.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ttthfxlf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3deuxvmks.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3noqmbpje.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kjvkgpqf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dpwvgtvj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bsobkqyi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uhesolmz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3plkzaqcr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3erptcwpn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bsrzvhta.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qfzmlrdb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ejgqwbus.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vxxqzyow.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ziygoila.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yhtjqszt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkrhnycl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sdlolguk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gcbjvklc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3iikmuyvb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqyqvvzg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udqwxrmt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkwdydbh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqwmcdhv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ikvtmpmg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dvyeaszt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvnmftda.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dqbrdbiu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltnydcvb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aiuzejzw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uaxabqyc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bbvzgzqn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3etxbnprd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kqrqtbbn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tlfpiijo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ydzebghr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3yzxyfkib.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ifnvaixx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mskxuzeo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ciuluqej.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xfndllrg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3idzqpidm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3smftlnrg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ivzlhtfa.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nexgrmfx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3elmoyphl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ogtctene.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3dlyaqhmu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ladvxbwx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3irfcyheh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nidenauv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lbpkpiqi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3eagzvfmh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3telmnmmg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mwhpghyj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ejbfxkyc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3caedjwss.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gaxufzue.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ojbjreek.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iayfetsu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kvvkpvym.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qgnftoar.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbetswlb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kxdznnso.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ktjriuyx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvrtulus.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uervvnbr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnfsuacd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsruiwaz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zeltrlon.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blmtudwl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpcuknln.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ubrwypfa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3coavgtag.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swubltro.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hpjvxxth.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3lebqmrbz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3hlducczr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rxfyspyw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rwkbwqft.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pclbrpcu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3llucyqxk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3qwybyrrb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3amwzunwi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3tevmbmur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvsmeldf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3yrkviuzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhitneim.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qzavvgcx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qiuqbrxq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3fqvezucq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xtqlxeko.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3oluueiuy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ziakuwrg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fptplngn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3sjihfpwk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3beiovznm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3mmxktlum.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3stnhzozr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3helnwazs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nsqosjsf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuchkhzw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fommhmxh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3flqsfhpj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wxodbxcq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3byaktdwd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dlwswerg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3htlscddn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pddauwzi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gssybibx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kwpsxipu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3yjovooym.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3kbxnzbue.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ffajfowp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ltrcyquu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3matowvyg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vsidisqn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wcfngmkz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fhqjnndi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkcyeefq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uznjbkll.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3edlcvsxy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fmtrxzse.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qwmaozxy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3pdvxoirt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gewyhjaw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pzyigopw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mwkgmkpi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yahjowju.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfqkxria.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qjkpobtf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ylsxftaa.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwrhsmjz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3brgvnyui.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3gluafcim.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3znzwwcgs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zirrlmse.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yncqewji.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cubzchfa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3yjpzsvaq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nwmnnpvj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ndjozkww.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3igydrnkz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3omvongnh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3wemfvijk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xfybeegv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aptfawqd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vkahqmno.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bvhaotms.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fkklzbvq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gynmsyci.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dfaakzma.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gzhotccc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bsvoxrrw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sttcyhrf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zebltqhs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gbbbdhmw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jtxgebia.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3pkpxwysc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3llsovkro.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mtzumwnv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3dfknarbe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3chmaldbr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hxzjtgfp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3lfexstty.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ufmykysi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nnubysdq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3twoomeuc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3czhvepuk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gvocgden.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qtwzfldy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pmbfvfgw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ezhmxvwr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dfdhinry.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dmelcbvm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3trdnuhik.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3swpiwcmt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ppgzylkg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kbneadcb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xbfweuac.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unqdpwgj.html


<!-- 参考信息 -->