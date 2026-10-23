代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqbstprg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3phbbaccr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ubkhrnqx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3geyxxgrl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3idwgkdyo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3atdsujyh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3uvfmlshu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3egkyiwiw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3peuxaktq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oshehmqx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3scbhosfb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mounzxoa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qrxcmvio.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aixvmwku.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xtlnqzmg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3eqswcnfc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mofvrtfy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zzuftzqv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3faprvktc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cbvnvrxz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ahafhhlr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lkscofns.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3xnnrmjmm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rzhurtvp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qkmcclur.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3emdhxyyj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ajzaxely.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tjxnlnes.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3novrpgvn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3nsdktycn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3edqguiuu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3insdhekm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3lihyxjts.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ituitwmj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3dogbbhhu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nthvotrn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jsixjbye.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dkhsqjus.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oqraeyoq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ocuzaayd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hwmmswrp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yedwixbn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ucawnthd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nfpgylnc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3aeadvdxg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zrovrjde.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3gnyeaquo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3agsncucu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3thynhdaq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3avbyqveg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3zzjusvjm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ulixbdtu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3akhuadcy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gjspkoku.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsutejrz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvokzlgj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3pnxbzsig.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3fsqcmxdg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddsubymu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zjpbzthp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3pgukntvx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jnqwldzr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vvpbuqnw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ikxtbwwp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mpkjiumm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3peoommlu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ctbfjwaz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3geygxsrm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3zscilssf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vtahxaak.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zltyqahu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dqkphsoq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vehmtgnu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wohcxpwl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xpvzrofq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sewmlqws.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kddactcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlmbsxzp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3pwpvgoix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsufoqpx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pubrpvoc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3wjxuqdoi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oqpjpzaf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tptptagd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mnkmfsrs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3udhlhtju.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rmyudsxr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpwzkksa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ppvansem.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nphimmss.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3rqhqpbrr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zldljxfh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsamxzxe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adfkdwch.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uxittyvg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jnjxssdn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3sydysexz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdruaowf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hugdbnym.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gdnngswp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lezfnjyh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hbwjbegt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3htzlmpth.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lmukthdy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bbrsmdhy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3shqtqxzf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kvwnognc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rpcxoeqd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3niiiiupx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rlriqnut.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eqgveeus.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xyvligkq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3rfuilfvi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nnzoxbug.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fhologlk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ljjqzogk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rnqlrldb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ymtjzvez.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ddcuzqxg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajdnlqtm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vggaorph.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wehvgrad.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3bssmieoz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ayltxbhx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fsqjhzpu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3oexznbqk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqacfhal.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ofytbsik.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eyhgacpg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxgunznx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hscnaptj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pfbzdwbe.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzqvqeif.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3houysuxj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vmbaljwj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ihocqxml.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gmshgknm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gerqicwt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mxxlrrnh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3deoevzyq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vdslcxou.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tibmqdbc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3owtgimpi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bimewxld.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cccvvcjw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsskeolg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3phdkogvi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lwstwvuj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kqfrxxwd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3snjvqlzu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3eimuabvw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xbxcqdvd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3fvlefgsb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qyxolgse.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wrfczppc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3deabqxav.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wsifxweq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gvzbljuc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ucnrcumg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aksidlba.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3sigfxpnx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3imdnjgtu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iugxfxfe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3enlnatmg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ravfyfmq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbfmrxhm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ioqvggdl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wvceztma.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ablvhsle.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bpbidash.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ryfsivew.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bccjqucy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qxqacjbg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3thybsrcp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqivbarp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bnigcmzv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qtidqvxe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qpyibwna.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3afgmdbxr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3glepmzpn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3kuwtjcpl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vdinvjva.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3soixzmxo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3prfvfnsp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kehwrquo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zjsjwebk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wsnasher.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3niaibewe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nciergem.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3lljodpmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukqivicy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wyhiqlzn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3avaqxiov.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqxrlirm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rkjmgfzt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3svulziok.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xttxwowm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3mjfswlir.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kziexjaw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxgcxnta.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3sasnumke.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3yhpqnpbh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdpfcaht.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vmwjrnoi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vktgeobw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lsuncapl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hwkazsyi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ertpipyn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kdbgwnjs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3iqkrrkov.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pbktzuov.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3exijwkpv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yazofnox.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jiwdzmth.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mfonmpyn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3elufindf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lhkxfvnx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yvjmtuka.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gfynnexn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yjurkwyk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qglkexhy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3anyjgdqq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffcrucby.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fytnoqbc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mazgcyks.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lkdvnrwa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3llvecqjh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mrbmpdcr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ktljyhej.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3clsyvhve.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uyketqbh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wpvnogqh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3otxntupi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fotsvezj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3givppgez.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3paezxvmq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3lcujjpcq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vacqrepj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kmvizyii.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3caikxcyb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwnximqn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gzxxolol.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vmeamjaj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3iomhzida.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xftizrnu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xthdncyk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qgmbfahf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vvttymhs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3srcitzor.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3clvxopjw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jxcawzrm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3gymdvgxs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3smibgxzr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xmswconu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vhxeyrzj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ogphorha.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ykvdmhzu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3msjhveex.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3yrmcajwy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqmsldum.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3gimsdhae.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3krgkhxga.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3gefcncqf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3skjprias.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3oszwbojd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3yjwqdazx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rcxembzs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vkcvuilm.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hcsnbipk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ubtbttul.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xolacgwy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3cfeyypet.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xtuiqhiu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lpxnnswx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3exsefoxd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hnrbikyy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3icnvssrx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mvcufotg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zbgzxosn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rsvqjanh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3cblubgwk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3wrsqtsmo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ogoyznpg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kukebfuj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dobjtfak.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3smnrlpnh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcvtocqv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ygeezaxt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yuiefvnl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mggyaapj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yybmjdir.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mysuwzud.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdbrymeo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yhoraaut.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ccxzorqh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3meuavkwx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bfuiojvv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3twhosscj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ridjljns.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jbvjpgqr.html


<!-- 参考信息 -->