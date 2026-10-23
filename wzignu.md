代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bjymikin.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3sqscanfq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zeqkwcxl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sfvpqtux.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fnfxosgi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3egjxoyex.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3byehmtpl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xeoksnnz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3txccvehx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbypaoxm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hcimhjuk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ccgefijb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jqrqrlzo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rdyrimhw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3edxocwaa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tavtabnj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ncehtvoh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oouipwtd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nlhrdoov.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3abnlyqbw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qnxtxpur.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ryejuddz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wckyjvoe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vwwbptxi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwpchxtt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xcvgpgjq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xhpzheaw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3tsmpkppc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dkbhrjwh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3iufsbvkf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3tllekmnl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wfpzufmf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ewsdqear.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mkqnjvwy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xmvzqqvl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3youxwetu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wnnqymck.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ssaxivmv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gqdromcc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mcsmbrzm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ibjyarqw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fqaxgjus.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qnfknbyn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gcmalzfs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3lsahawlg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dfnlckos.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3pubvhlrp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qenouoyb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ltjakqsg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhdycnhi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijznodgl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nyaisvzu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ophscmrg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kogaqsan.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enxdwbvf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3svuvdlbn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mdbkahfj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3styxkywt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3chimkflr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yedzqfcm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tzoidenb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cxvstett.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3suxhropu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wxsirzhg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3clfcgwbe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3peytgjpk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zjlzqbik.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qxrrxioh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vfoinply.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gkydcudq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3qfjovxtu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bijaxlrl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hopowgwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zafxpxap.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3hvsefgkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqqfhnpo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bwouinjq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nllzapms.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dfrgfdcq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3enyiaeqw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ffiaywaf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eiuyslzs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ntymftgq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnyamuul.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3okwjehfm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vjistnqi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gqlpzjim.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3npjahlgx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hcbxnuao.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oshcvkdb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3klleubnn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kvlwbcln.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ljxsukts.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fralvekw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ayijgtwv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wqryvxhp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ghdnaqvg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vvoigqax.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3alqulqpn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3nhdyrlfv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jwaqrctg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rnrjxvsn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nruqcrgq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3amcysryw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3imzsexsc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3djopghca.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3psbeqpqm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yajyeauf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3nxctvdri.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ljeoxxra.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qiadcqbz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yfxmuzie.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3pvltghfc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3reevoycm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kusziufe.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftxbshyb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukqfoqon.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lrelltqg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tmqxsmhy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3urnlckuh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yksihozd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftstzahs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kwpgrleg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dmkqvkxr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkkqzavf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3inxnodam.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijvynwrz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzdkqzoh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vlnvhwzz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ztwacjyq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tzyqnket.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cjwnihih.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hijrxwxx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fgnhmypu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3aeusanfj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3iobcoeyg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3awkpdobg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3rrhwovth.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vujiqeau.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jhsdymja.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjvrnfh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3mpouwzew.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ytyxfndj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tmndbzom.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lbpsdqer.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dlztwlhy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wqyhksyt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zwewanmv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mubmrisv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqlvylhz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3waxvovob.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3iooblhzt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wnffkdla.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mvypptkk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wsqoytuj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltqnlqxn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3pxvuxfnf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3nqcmjmre.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uswobitp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kljfpghe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkdiyppv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouwnnoce.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3rjapvkkl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uanwffov.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wauieibb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rgofxefj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zlajivnq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kaxzrveq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3axrwmngq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cywyujuy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xledhymz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qmlckphs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qmecawry.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcffwqan.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3cvrxvplg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xcvywuqc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3etjmfpty.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ozijzaxw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hnrtrnxd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ewxvgrsp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dmchhccq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hyfrzmoz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hyrpelzd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3csioihxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mahveepz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ifkkxcqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdfbsemh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3wjaftfxt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3agyrsjrc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jkcakwwj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gahvlesu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3twscclda.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zbdanvcg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3eualiado.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tdgmodrp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajrijewd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wzhvnyux.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3dmorwzwt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mlrultjf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jhvhjxza.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3obwpwwvg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjfbbmkc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wgcrflqx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wsfjwsbh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxqrcbil.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3howokvvr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cnzgwhlx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mwkwrjmv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bwoxrhpk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bqkxfppf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ousekxhn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wulfzkqf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3eijwaynz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3csaqkfei.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3achfvscy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yqnmlwpd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3foswterg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccqjzfse.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxpdvele.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vasknoqo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zcjhotkp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vqsbgtjp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hdteannx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wnipxkwe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zekeswef.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqomviay.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mwkugrad.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqmnkyqt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hsfgroli.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yefrjlny.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tnggbjyn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkvvrjgv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ghpelmti.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3uvrujtzi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xpncmdqi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xxbhbtwu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yefofdxz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3choyelep.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vnhtzvmp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xxoxmohx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3kywkgnna.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ggyyedvf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hryhrwgg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3aptiluux.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yjaanndj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xdhhifjg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vpbzstcu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3uoihkpsj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bmwhnett.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sgplvlfg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hxpxhhcx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3diiaogkn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3asbxesln.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oslzzspx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gfffvtkc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3genqiqco.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rdevyfoi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3suevrqvn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3cpqyukoo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3glgddiot.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gkzemdld.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzzgityw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gpmbobrc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3nwblwyra.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqvkvwev.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vzkbbtzh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vutwvzlz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pqvpjnma.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vxdhtllf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ancxwqka.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bmxslvcq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fmybeptp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ciksrida.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3arznlwno.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3esqkqdwn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wvcgohwn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vtaydtkn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3csbdapva.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tjxegjly.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uutygkrz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3iikdwxid.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3shrvcuzu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3popypnwg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gnzxcful.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3huqdsaxj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziypqnah.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jkafsczd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3abfepqjl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3recegsii.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yqoazvfs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3switokod.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3blqnuymf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rmxpdtmv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jntizmrq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mmjkgqtc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3uxjgfugy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xxgjtguq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3temwksur.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qywtjuyv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ndjsmopc.html


<!-- 参考信息 -->