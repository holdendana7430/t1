代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfbsnesm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pauqasgh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ocsfedyu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zfmhasfv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2uymwhndi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wawsioop.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kpqzjqfl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jpdamzyy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2cpcxbyyy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zwzutsud.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hxqgcdzl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ohtgfvwa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qhnbxlhh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2cvykqgmp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aqtgewdh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pkeymxrq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvdileup.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ubierhal.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2acetpfdw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2krutycpr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xkfhjjtn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxkzleaj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tqvlhigc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kzsjmdxp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qukcbfah.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pilsrilm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vaizdwdo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2minvjjyu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lgjijsth.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mvpcwift.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vqjnjucc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2iyildxyn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bjbeqsxf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2eokffunr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivgnmzib.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjoajwbp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2lftkakzv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cbffhfgs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tcmyztzv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tvjaoxjo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bbvpuoax.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2egluysgd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2quzeknqy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2micvmjxy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aizbysqy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cwxuesfj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hqzbifeh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2gvymiqqc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2umsqmhrh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2drtxcibb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rtamvlwi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wzoeqzsj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ueqieglk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vylqguvi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xpvgsijn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2yxtjrytv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2pgrhqjpz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2oxrmmkyq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ubmmzibw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2vqczfmzs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2laizqgtl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2bjqlbwia.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyowhxto.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rsqqampp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2trzlvqys.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nyrmteuu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2zgmstojo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2csgbygjg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2prcnsipk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2poqwqffd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oybvgshc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gwirlbvx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cnpqyicp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wxpykhsc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2flfugtub.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ljhdmeem.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2kcvhdjhd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxqwswpx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2edojsedx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ekipvmng.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rghvbbqw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nxsqjyrh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hprcwmdy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ozuyvnjm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fxbrbhku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llpexvow.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jerwmwlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrxlppbh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2plnrassm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2trnkspwl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yinqpxhx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wfvwhnfk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dotszwif.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vfryemwz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2yocumzto.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozmqbnpe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pwcjcdre.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ratcrrre.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jjsusakh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rktjoqff.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugpleqdj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htzdedzp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2amcajztg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2tvnfmjhy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2wodqwyeu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gquokldu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2oysmsewb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bhuxhtzq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gxxttojq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rlelflxo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nlbfztww.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ikidmdae.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2guytmzkl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2bmuvzaqo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mhqrbojs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bntekjzc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zmlxwosa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pdlhgmsq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fnfkfmyb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hrklbmak.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lqqdbbdb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ggjvxnnj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dvmrxueu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kutoqlqg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2eadbdipt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bxqomeca.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ttedwilj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hmmjnvvz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ecvoyrrm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fckfzqoq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2nqyxmhfd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jifvirpl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmjtgrny.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cikjpihy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yojgeckf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wbrxbdnv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjdyrnxt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syshzqyd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fthkbzmq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvkfusct.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2broarwcc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hdcjyejr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hbgdmwjt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vowgzzbl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gkrigrpg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qtbmvlqh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2iimtdqus.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2luugrzqa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2eozugagb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2duhurfir.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2pavrltkc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fyogwtov.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2myxchdqt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kzapjohj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qvxudktl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xdramoyb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2okfdsadp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ihabcjxb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jqvvlwao.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aisebgtd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2lstvzgub.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rijoxaiz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jzybpnnj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jzszgyhq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dlwmgher.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fdsfmsdr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zxglapbw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lctpvqkr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ngazwkeq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2pympatuv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gladxzyv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mzapizeu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ercxahqj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2irlwsxoi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gvgmtnud.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fczoxgsu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvwlmizc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2btktvknp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2tbfoxiqk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfwsyhoy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2twtrctcu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2drruuyvp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2toczdrkw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2elaaojxw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2pesvlsow.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qymtixpi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hxarjfgo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2aiixmcav.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zbtmhblq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xsjpmvyk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2eevdxpld.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2byyzwcva.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qiephsjj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rvsewssc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vdsftvhh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uiyyozqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2biobedif.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pziscikd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxlzwllx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2bymthfgf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hozymrpa.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2geeypakm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2upaqyggj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkqueyai.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2laqvdhzh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mzdvbvoi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ayxizozv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2reomhqmb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xuwqtvrc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2oyizixyv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qsmgwzgm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2irfmevcs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfjompff.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zwpojvxs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2mfayqdtz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2bcfkbtzv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2inynpdym.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yhmtupdb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sopylwnv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pmuwmjxn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gjkddtut.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2khgxglvl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zckfmxoz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dvyowlox.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cfynishu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mvotadcu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2logppryf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gpngnhki.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcnkoaxz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rypwafyx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vrpriccf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fiprfbfn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pyneqokn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ysbtqxgb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hcmxahbj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yvrpftxq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vpxkfztk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xmlgsziy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewxgdwxj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2baujzplf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tjbqfrnv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ahoaroez.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ksapjtyq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rpptjssg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wlsysvpx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zprlzvdy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xghxwwpf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxutoqzu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2muuxrovm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiklophl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rqqxuqev.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2cfadjyof.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2nwlmxikm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2sywslkar.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2beglyanu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2nkcruekh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mifnjaoo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jsuggzow.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iilujzly.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2igwuwvyi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fmyerrym.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gxcfzjxv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2skuxkwsb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gvgdqgft.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2attngbiv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2svprustl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2sfpxyvjo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmlwpkbj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2weywhmtm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2plmnfbur.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nhjwsknw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2trmqvofe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2dlqkmvay.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgezeehp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2pgbibnoj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vszvtaus.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kubqiqyu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ludtcsma.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wpdrtwkt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnfllhhf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2pqndthtj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wioqfypu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qjtwrucu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2djawnokn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vncrdzjv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2rvfcoxzp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zzzqxual.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bjhedcjk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zrxtjzrc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2apjnbfyf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2etlccdcd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dzobldqe.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbykjusn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2olkszjjm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kzljopfw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cwsxyudv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kpjzahou.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rdogmtah.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2liwmtlnd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ielsarcp.html


<!-- 参考信息 -->