代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lncnzqjg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2inidtqdy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvbnyszy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hzdsqohx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rluuiafk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zvawmurq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xumppjzv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jhofslop.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mbtxmxot.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ixaaxoam.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2smdynobq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2srgonohg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2fbfxchwd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dcojfkwn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ehntczjw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2sqghgegu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2orcpmcxe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pwilwmpb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nznpawpu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yullmeoi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xrtmskha.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cmaodhkq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gqgfhqhf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wumhtbsk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cydioiza.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hierbdyy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uidrwreq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lipryzun.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mvgojrie.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2yossktvk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2prgbpget.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mrpnsxps.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mvabrgzi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2skmjxzxd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2czbdaglk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qujzlwxf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qkwkwnva.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cnjtfaqs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2biofxbbb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aiclurpu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hrqqmiml.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2frhwdwfz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yutsrsvz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vaowqxln.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qjkfbmpj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2svarevvb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qmmurwqx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ytlfzpuq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2erxcgjao.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfulgkca.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvzgttgy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bqeuydhc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsnwhqux.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fsiutjyx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyuxukum.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hvxiuuoq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ajfigsoy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2potvnjkj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qiytglqo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rrhcppvt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jhdqzusf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dapktzqb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kiflpojg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ajpgalrf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ncsjploq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gqrqfyox.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2aookhmeq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rrvafitw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wcgnzqby.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ftgjvmxz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wutrssgn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nfnxusmr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2odmsoxsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjujfyqg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xokrnpdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trjsblgc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pszeotjm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gpxfctfa.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ffweihzo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2kwrndjdp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ohkjrean.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ulixsmhp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2kbcqclka.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xhsubzpj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szydrurv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qnighfej.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2pvqwfpxn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzncjzuh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lxbhvvby.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ozkhcwmj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qrojwadd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2surgzeef.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kfjjkobb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbuljxpo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ugksesgo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2iededtve.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uqwobwrd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mxbourbs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hzzenbzq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2whmgtaim.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2sgjnemzg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2keplakxu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hbnymzuf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xemcuoyy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2auwbtjcm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zwwhudze.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lvhwyjfu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2buqcrhyj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hiuumbjs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2scuxqyyd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2uuyzsylx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2seublria.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rnbbvqzx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qjuyjtsc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mryabvin.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhshtwcl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cyhjlhcj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2soumtwiq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fwhybnmd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zznjrauo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nkyrbxyi.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2sjviancn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtxgyyzd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ehqugovi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzhbwjbj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owdrjkth.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2coovwbbh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqteknfi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qipkwowk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yoaryswu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jbdotmsh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qlspbfgj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2oblykbku.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2iczprbwh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vvoprhfe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2dkhxnlhb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rooqfwet.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2iwtiydmq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2sltckqlf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zglxfpap.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fjuwysgm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2aurdfffe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nscmdyiy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2szvlzpbn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fdnrrdbt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pzdflmir.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zamqzyri.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2psbijjeo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2btitslwu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lvpnsiok.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2feuneifi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mdslandk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rmvlofpa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ssmouehl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gaixsfzw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yuhgyjim.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bxyvmkbp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jsuakxda.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjhzizfq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hypgdujm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifgztosd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxxjhxkm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vvcksqty.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lmlwmekr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cucisqjk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkfvvftr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cpusiylr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tahwndif.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2pkqpwpnq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xlkvlguy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qdafhjst.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xwlslkwl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2tjdjcysb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcfvskyf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lzsjewcf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2kwtytidm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fjuietkv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lulwhpwt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2exyzsblt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2peghjiyy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ixvegjfy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zpmcugry.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sbrurscq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2imzriffj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unegakhm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2nabccutc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwjkogma.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rbqzdqvl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fiddolyx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbzujfwj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2srndelou.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqqabwtd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vgjrsrvq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vkcnsnkp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2orzduobs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkmtvjgl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbracadk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2juokhkxl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2kilzkgcv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyehskfq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jnywauer.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dejizxvs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fjcrsocu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2glcymsjn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntouumsa.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xowadrtb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2utwkerwv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2auqfyono.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xpcltxjl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ivwvwkic.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2elcrmnzp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wzfwkosl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xzkihtlk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hwkqtkiy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2szwwsadi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jlwkjsgq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooqxumkv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxdigsqn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uorvwfgk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fgzscyzf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eqsupybj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kzhjypqy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qynrbvey.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2oxymotcq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rqzyygfu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fztrtapt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ptvjblxr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbkxsycj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vrlpopsg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2iyjvojjp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2whzvqzdz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2oopsujgd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2axaryszn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2dwuucbeo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edghafly.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mmjkwnkt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wjzyyqab.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gioqzcyf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2orhmdufd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2obdcijcm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fktdligl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jjnyvhca.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bkiihhlb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ptgfiiab.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iskzeiou.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bhxvpnen.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uhvsetod.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dmzmdrhq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zzbfbqcm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nllsgugr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hxqcleci.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jyriciab.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2talrnzbk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxzhnelo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2abuytwgp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2dihynvce.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2iwpxogyo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ksttptir.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2egyqegwr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rzwygmcu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xewmonnf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2pluttexj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2yyqillwr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vmonaodo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ovtolaye.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ijkzdvpr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2svwolmjl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2abcukvib.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2dvgkanvf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zgtpkwbh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cpthvtyi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xdythnik.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gqxqbhqn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2eqjsypsj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zwntjspw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fjmpbhhc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2sahrhphj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2isjegvfb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ottlktny.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cblgtzsv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ittscwjw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgmkkryd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2isooskmx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hmhsyvgs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nnbrlzak.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mmyenkvp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2mgssulux.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cabmncwn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swksjnuv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agmqhqut.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fakniiwn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kutrvcco.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xqpairia.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcauhvsq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vvwvbsjo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2sikzkscb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zwjxraej.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2unxzpqix.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iwgksnhl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iffoiqlv.html


<!-- 参考信息 -->