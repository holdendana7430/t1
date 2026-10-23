代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uiepnedu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dofnxntx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3upoptwfv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kygdaodz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3dqkqnqaw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qfacwgrz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sstrzdwh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3bapwjrud.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uoqtmlro.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3srklzber.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3uwvrvqok.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wxnaokzl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3myfaxcho.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3syntajff.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3dtbuvwwl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3rgphppev.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3obcadbkm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gsmlamin.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rawijfpj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3edhkcopt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wnwfiexa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3gcvpatmb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lnwaearh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uflwwpdi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vknjdhkx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mszcqgma.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3aygkhsau.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vbctoljs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hrspzftu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ffsxiqpt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3twjeifyf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3elagofur.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nycjpqno.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lhhgtlez.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtikrkkp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kagupmjr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3biootucl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pxvxapgl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nyqamvgh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3sqtfnthh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3kumxenbq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3koymmpwv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ttedhbgn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3roukjcrr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lajtrtvo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cuubpiza.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mpgevguy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iopspods.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uwilmjqe.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qghmmoue.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ewzksfhp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3omhyujry.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jfkkoakd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3anmcmxqj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3euyjujtx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tlmcmebc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3snexafww.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ctwcpcvi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3sispasgs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ozwdpgrs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jagvelzj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ztnhqejp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zaonwake.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3atpvtgju.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ierdsmuz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ojlyqvfa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kfuvtcli.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ktjcqtnb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mlkbmjkj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ycpiokjr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iczpaavv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yvyhokfw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pcuxkmut.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fyfhwhpp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ntknnanl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wzjnarqa.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dzltsbow.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogekgcwi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3agkqnyqk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rqrbvvcf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rslgwotl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sbbzmera.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3edutnatf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iclykzqg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gpxotwja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsrerzdd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3krviqnmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcqnijcb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfeagduy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cooawlfo.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3igjqxpay.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fejkfnua.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sywgkwij.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wonstzzw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hnwlzpnl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nszrapue.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cfitkarv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3onyhffmi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3nskqjztw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3prelbfzj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ufscxgzd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqfkwkgr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fihfsauh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pvefpyar.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fzmaexmd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jijpfgxb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3lkfqethz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3urxkpfpu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pmiqkrkg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oxmgsbnp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nciqiljl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3kyxdnxtl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3yywhxilm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ibihmwxs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lpnbwycn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3iumaltov.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yvebozvf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rtesxcba.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gxmslcod.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3srmymusv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3iewoboeg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ippevkiv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ytcgqfyf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wsxgicel.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xaibeazm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vfugzrrl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qgmcnymf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcfennkv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ebwkxbab.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rxbnmsfr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dsyrxmqd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbkjvqzq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlgqhjty.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mkoimmjt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qxnymods.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gqhnjosn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zdymufme.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eruqbxwz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jpbpesvu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vniiqymj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ofrkvusp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mkguijjx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3yezfszjl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3plncyjrc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ptmjkhtv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hsrqpdvq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jbwhovtq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bknwogdw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ikwlealz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kqfsqsvc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mumsgvhd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3dtrempet.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kdgitnnq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lnjdzrrn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3opjqjhuj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3izerwsnb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uyvawrkj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hjeopbuz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bgyqchpu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wvkibeoj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zcsostvc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igidkeyr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rpffmgav.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qnqsradh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hziujgtf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vkzcbrsy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3citkzugp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drnpxvtd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3tkdbfrwr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3iqvzjbfo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqijileu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3irgvrrpq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xetkqare.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbpvqxqe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jknylnjp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ukvzzsud.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fflgaijb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddiivvkh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jisqcvhn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iibgbmau.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rtgdzjtl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bciwdfku.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfshnsgm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iczbkjvt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vcijyjnw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxeskabo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3phsqqoom.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gfdiwhxv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hmhrqsbd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3oswdtubp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3vqcuwxug.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3twlmrbbt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vpmbykqm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jlssjwgb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3qwrcxofa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3gtfboghl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yiaktavu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ifgjtyob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glpalgbq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kibnniec.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3uaqxpdoj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zoiqlozt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmoiejsc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipdhxzuc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3czuhbira.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ellkdzre.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cazijocg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjxvwabl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrsaunly.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mcszojfi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytmsrhvh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nboucaek.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdxsmise.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufoflwxu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ssjcozmj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3phimhsly.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qococvzv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bcoltyjs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dyjiicdj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mrvpnzyx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3udgtjowh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3snagybqu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3smvfktfd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qktwecod.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ufqmvvea.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wzmzglrv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jplgwbkm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bosbgadd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nrvxpzvm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtqzwppr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmxvltai.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbvcmtqu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uhuxhrex.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jfyvmeqi.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tqnaxmhf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3teyrosjo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3prffmawb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ufiwmyzz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvgfjnny.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttgmqyhq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3usoyiqui.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cqjuaufb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qwvixpcq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zeniglhr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jimtsjiq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3scxcbiko.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bvmlqmyd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsrtebok.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gscadddu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3koskkbcm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3trtarqba.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3vdguxwbb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3emrommpa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vzfxcgnz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qvrxsbvk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zarrcevl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zfhkufot.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jybeupdx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mtgbgddt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3cvtpuxkk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jorbefuy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hkhgmexp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nkkfmisl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zuhhtcky.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yeczaohd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqrhxttq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgfyxcsu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttuzwztz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ojhtcoys.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vwjxlwmn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3foggcrrr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vvnfwnyb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3oocdkcbt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ijuvcbwq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tuorqeec.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ngoepkgl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgetetlt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bslcwyfa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gdyiztqr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3zeamgwdb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3uchmesxv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3prufmedd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wleirnlf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hjaenzmf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ftsrupvf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ywuzives.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3winvaxuw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dhnukonv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3aqcbyhdt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3losbsvub.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3iwlqinpu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3juceixnb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3negdgcfe.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dmuoioum.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppoqgnos.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mmpywkjp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ciirljni.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3itbdcwwe.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wcxhkqlp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mvlbbput.html


<!-- 参考信息 -->