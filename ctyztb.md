代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lvlusord.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pesxkrxe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlhedvaj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qiggwexi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yzfvhuqx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fxvylpot.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2murjrrhn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gppslddg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dckxywve.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2zvrekyxe.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2aifzjkqq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vnafkhqq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2hwejzqzz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gdjrwjuc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tzixxhnf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qaqgikzz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wfahpxxj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2asjnskkk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2blrzsqms.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sxmlcbeg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2gtfkmknd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dznkwotb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zfldtqcv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpuushn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wpirfbxw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2siltzmoo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gnwtseul.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zhwnryob.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qjlaafaf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2nsekblgp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vzeohxwt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vsiqakjf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zmcpfsgy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oiowzqxw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqxyjkid.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cxpbsqez.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yxfgtwte.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2syrtthjm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vahqllpo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yhvannjo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yyrfopsn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uylgmkmp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2bqzqigcl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2erybpyfd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bwytdmap.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2pschafth.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2apsfkayd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2cojaxzhv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rptyxdhb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ogeokcsf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxkpwpty.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2njewwbcs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmwrijug.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cnrpkcyr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttdlvrsx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2whjxtncj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2sikxolcq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fatdcvhk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sbctwpit.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2guulpgvj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2spvsrbvh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qrriuuxp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bhzxfrgi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xsqrcxgo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cqolrwis.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2fqglzrfi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yvzretdo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pfibqdum.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iobvqelf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2patibwbk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ehxxotdu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ouyxyrda.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jyeelbxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqcwlcxi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zoknesdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zagvrjim.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vdmpucsz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ympabdoj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ejiqofxs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2etfdwzeg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nuwrpyrg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ohxzxyvu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2noirnkfc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tieallfd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ukcsamsx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2sbzdacyd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2mwaorcbk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2hcbqxmnx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wvsxsbeb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2szfsdadm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kucfdcfc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bbpivmue.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ylsrdzkt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hwxjhjle.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vnkmtuks.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aweynphv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gboaeeyi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sehucrqo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iyfyjnim.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qevlnhnw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2oiffsgse.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ppvdmzbk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ajksnlch.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nvjnjrbi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uelqfvcw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pjfrxqxl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uwxocbkv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aewmnxqk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2eyodkiox.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yobxcriy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wbegvnql.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zslhnqrc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ffzwyeil.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2eqbgzlar.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qfofcrrw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohqhbhmj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pztxwluz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2huevjtsc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2glbdemxs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilmhfwiw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lilucjaa.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dtnzloox.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbwunifi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bsyaszmy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etxvcezb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cumssraq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gzmqdeba.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksfizfwp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcgmhrji.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jjqdleze.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rttmfasg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bxoiwiea.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2erllhfdb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wladfyjj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jdbgqreq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ipjzxrja.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mnviuvao.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pzayvczf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2poveuadu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2igogjnsy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xtwddgqz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2sxpmhhgb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wfkelfml.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zjcxfxbu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fgoeersc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tyebbpkj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2goefbzye.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gxzaadze.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jmebclqo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2livoijlt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2duphpxzd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2imugxovn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ldxrycxr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rrtkwlrh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zulwpnab.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rucebfzy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xpkhclwn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fgqkyrzc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nrfsuucm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gbylbyqa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nklthumz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmzckjjm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wwkfxlid.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eekgrawi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lzytcovt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtqmymut.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hytxhxje.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wodyjzzc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2pmsvaxed.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhxlyvqx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2epjgbfic.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ajwduexk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hembgnpy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hruahour.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hpwkvxxi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2neldgcqm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2umaygtit.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2euvvgtnr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2afypahmq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dxkcwyop.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wiosuura.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2kkyxnhan.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2nligzqve.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2degsiaqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jnuahzis.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gnvpnqga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufkndiiq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2hwhawddx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2arusdqnd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wfchsoyq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwkqjrzx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2khnyzrlz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvvghlta.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mtxlnsue.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bqeygwae.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xwcsdxnx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jzmwbywv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2locegzqc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mtxczdsq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwjofxqw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjctuifr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hionnqur.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lqyjhftq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rsfkxdrc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bhnobmju.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gwyuonwy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aciosmcs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2levxcokl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ekllgmoj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2obrpfmww.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2orkjvunc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2trwdqarn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lyqoaimr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vhjoijxt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2pgteelnp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cmkklmay.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wqkgaehc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrufwuqe.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2feehuxiw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nfrgqjkv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qttokhxe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mucqapkq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pvyyfzjj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2mlozgpil.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ujknkdlq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jaxzldqz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vajscuug.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvrowpym.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2igawibxz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fggrkxca.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2upievzka.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyixvvwd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2cxlhthln.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2tjjiguqd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rzgwyxtu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxsdemdu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ustuxjza.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eeaplvpp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tfzbpzga.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gprqrggf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2uaobmeir.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vlqkphqw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2etgzaddn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rzkworsb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ypfdxunw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mxzdfwcz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jiawzqog.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mqvkjniw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fvgszrsf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tiaerzou.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bognkdnm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xmuzvmrz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2katddqrr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2cinlakmf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qwxyctds.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2crjtciwq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zccxpvtw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2frndfjcy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkxtpptc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ckwskjmh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2nftlcngt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2svjlidqt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zlywdfvq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpfhbrog.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nelkpadc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2sgeqcpbd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fotzocbr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibsjjsqg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fwfohtam.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2okwdpqpb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oflsgytt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zefcyoce.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2msmbjxdu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pxxmrvpw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2rbpaibrq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gaqcaoxt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2qfuvcman.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2gknkkupe.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2aiovlbti.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lcnhkutb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bhtqpour.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2eqjlgpjr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnlhtowz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dijlidmt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2krptjuoi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2iuipcveb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2nhkrfjqf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gfwcsdxg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgrrnekl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2czjmiqvv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qufnkgef.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iafixpoy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nnxbtkmc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2eikpwycg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uocfwtuj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tgyyokbb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vbirxadc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ckxvhajl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ufpznmjx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hejfkjgl.html


<!-- 参考信息 -->