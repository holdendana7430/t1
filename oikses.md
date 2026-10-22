代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2sivepdly.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bhkytdip.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pyjsbmnh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vontvvzq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ojjccxlo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rvtwnspy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mxiwpyfi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qsykylva.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zaxhxgry.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2pmlebosa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2iovmliyq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2hiodiezf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwfrlaph.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vfkfczmz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2apdfleav.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zpsoixzh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gadbuzhp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2sippuxyi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iwjbwodz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ekushxpk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yoahrhpg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2henngpyv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pkrpjxra.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mmxorfvk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2hcozzmhb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2bkmfnzfh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nroykxct.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qoyyahlj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qrbelfgy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2prdqjntw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qdjiglox.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2olhokjgm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fbqbpzav.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zbmghwmp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2alviudoy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2slyhlpic.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2thxlucqf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2kxgvgpvk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvphqsg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ocdlblpo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2fkfskeep.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lafjabki.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dteptufp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ceshgdcb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2yrqxntgs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qzewosni.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lumkytqf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ebvhogdh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fhhavzbt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fwfmssgv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gyplpaej.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qjxopoxt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2awhohekx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nugomgwd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gmnjnhen.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wlswcsnr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rmuwdjcm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jpappnmh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ebiaojqu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2weosurjy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xvhuemzd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2aicuscjs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2agyqukvt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mavauwfn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jswypspu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbyesihi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgqvdlob.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spovsdaz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2owoxqohs.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ocadtybe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgmtvmdl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wclppkdc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bbpeawrd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mmtwnnaz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qnviwqks.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rrlwrfqs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uvvmhutb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kzssilzz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nkcpvbzx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zcckgxpz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2pvaeqcnw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vzlukasj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2anucuniw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iyanbzux.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zqbkjxes.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dlailolw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2enlaossz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kndrdexs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2uputfsym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnkkmlbd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uavgrahy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yorlinru.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhjrqxtt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2phmizacl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fjbeconx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2pbrmvvxi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hdpmvnde.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dnjvzxmy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2sawbqiqh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncjdhhom.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fcvdfizj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbozafch.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xnxjnfoo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2hvyjbdpk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xopgfplt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2phoxfzqt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ubztmdnq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uzhipfye.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2geitenyc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2lvprgrdj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gxbyorvx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sqpwfvcm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fkrbsesq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2slbrxotv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rcnktmgq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dfwbifrv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2doaiqdbn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ikaypcas.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ofcyuhlt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2sdvheamf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xoborcie.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2hwfzvflr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eyuxqeyf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2klnlblud.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wixgltrk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ywnewrik.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qjxrwuml.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ufjtcryu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bxlnxvvq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cbjpdjhw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dvzfkjey.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ohftrrvw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eevgbqiy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uqjfbaut.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2sjhnltmf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bcvbrwej.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2folwjqtz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ctjkgcjl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2isfzpxit.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bymngmum.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tuorzvpa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2poycvciv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fewhummw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdldhzzw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnruzoiu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tbnicpwk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jtyqcvkj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xljdnduw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hpumqpev.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2phizhncb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gaovskqg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ucoqmkax.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zpqdvilh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ivseiskv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2fosmrnhr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2hytpaoju.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dsymghwv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qcgismnz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ziydipfk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2btdpuezl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2aklkqgwz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zaprllcf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ynwvdjam.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2njobnvfg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2skzaemcq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnctaboa.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jefuvryn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lyotulyn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rcocnuft.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vzahvltr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2muwkfbjs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bybblalt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xjxgnyia.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ptwrqvcu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcskvxno.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gxusuqnm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2beqgcyfo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfsvucms.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dlhnkxwu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nyhwizdu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwoxjsru.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhgnjmru.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vxgzmnbt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zxrhkmos.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yupjfvjg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwbmozsv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2udzmptmc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qbgkxxuj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2famfbmgr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjryseja.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2tnsepsom.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jkiiuwqw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2szidzanm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ldgpjwdo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qncmwoir.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bxcaharq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2twvacber.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2twyenotz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ymisblun.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lhzouqao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsgicwrq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ikxpnktl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opdbeepf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2knfbwxxc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zyqlnaqj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtbbbxah.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekpyvneu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hruszssk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqtbszli.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2apoizfug.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2codzmiuf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2owvnekuo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2quuneolu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wgwxxtpz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbrefrzz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nipfttsg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2creonaim.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2juegjuys.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2eazzgvxc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2aoxtqocl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdrgpopg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vqtfzoum.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xvmdzpdw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vsvbtxrx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ezqgeujk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qjstzavs.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ndivwqdt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hplapgpq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zdeuieif.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qouzucpr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2shbxbftm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ckqczyuk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxeendtp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbkfkmxd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gmxzyluf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mppbjslr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hhpatcdv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfthbmxk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xznnfgyk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gupozqqe.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2pxvwkzlh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnvwbzme.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tsnkcqzf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfbgaqkm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxdsyeuz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2baqxrlir.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2uwcemmkg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hravomtw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kufylgvx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2flbazuyz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlhkntzw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwayeqkp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mmkswycw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtddasoo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2yrtvtxcw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2igynffwt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jbyydntr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rqztiwda.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2uycjqtkc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gpglcljg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ekgotcsh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2inwkxugc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xhphevpk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2jdgjkoup.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2cekzkxlk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wsgvpsjr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2masseshc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2efgigxhc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwimiyyc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nfqlmtlq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqmjvqnv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2shlfqmus.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ysyoqebz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ruehcanm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cuwmepid.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fexdygas.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ylrhpegv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2evokriuu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fonsssti.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2trvxivxp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ozwoknmt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ywddvarl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xcymsohu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2aqlunmbv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qovstjhm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pqqllqio.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ckvgzltb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2vjsjdzek.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jdkustaz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2eswblnlm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2witpgdnc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bkffajue.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xssgfssl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2czjnaklr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2yzwpyjuh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cqlwqtgj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vksryjlq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmayanee.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mxgggpuz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xhmjvxbl.html


<!-- 参考信息 -->