代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whzyrwrf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hdibrqmd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3dnwghufw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3uwshoann.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqutibhf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmznozuh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dvwyfiwu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3iyuzmebp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gvecgler.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hmimejck.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hqwexmmq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qpgagewi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jrzqfyil.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rrfwubuf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3lwiojvda.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qvvcarci.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mfswheaq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3imaizdpx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3djzoevbl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cczaeozg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3xuvdnxjk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tnhdehqb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bkanlhmr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hynxcaxe.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cuygkkbx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zojkmylt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bnzzesln.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cfoegnjv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iiuganju.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wtgivrob.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ecmftemj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3vhylzwsd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ffbnerre.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zbtzvilz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lkkiezvb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3djslarwt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vshehibd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bgdfqvgs.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rrhuufnh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lphizrei.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3elolvafa.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3okcdgopt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3damfbfha.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jaqnnyop.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ggtsmpoq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymlgczav.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vskbscwm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3exblcxwt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3axwlevew.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qdklqsyl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxiqyflg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3pvgntqnv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jgfudwgo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tiklgvrn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3voyoivir.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3erffgnys.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rlnbawje.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hypugtnp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pqifmrjj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zvnxxwqh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rnrxgkid.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnubowwh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nfzmlqpy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3urejwuod.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dyzclmhv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cqjjygeu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3olyegvyp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ychutzmu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jifpjspx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgiwxptz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3uthascfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwrpqjad.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3msymrrov.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ddxrwwru.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yqxjzive.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3widcgsbp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qezvsdti.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aqfcrgqj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wrppczzv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgpkuplk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rpseatan.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rrzivofa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3cfliufcd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqodyuym.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ebrreabx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gbnrzbcj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3odjrlbpn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ztocqlrx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hcuzdgxn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qcfpsyuq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zrjvcfrn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3lpvhevjy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jzoupesz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dqxcjlbt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3slhhkvav.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jqfblohn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ykwglsbr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rpviqdke.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nhjfjlrq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3dygmiuuq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mvbtbhfc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3khenjjie.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vzlmhghi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jfhgzbmd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3husnjise.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oastiocg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dokskedw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fdojuanf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vjyelztp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zdepvbih.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pbnptwyz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqzzexfa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onyyeelx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uldbvjni.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pgtqvmen.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xdfhmdku.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhuzyugh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfvmucme.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fqnhdqbe.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3skgblyrr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evnjjmcg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qnaiezsn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wghhymuw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejfehbpi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckvtpowq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gqgswuws.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3fxjmcikd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uckzmbjw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3oksivnte.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yubytfwq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rbazmlli.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vqzygecg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pkalcqdv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3pvagojek.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vimhgrub.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xiipxewp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vrtdnlwj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zqrljqpk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ntvwmbly.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fljvirju.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3omtpyotn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zqibhsmi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3plpledse.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ikipaxkd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3quirguzf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbxbsqhj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wkqxwzku.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3soqxhrtv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uhfxeyuw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3baznyhvk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kdtgkbjd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awozawid.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3edrsmrnj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3phjaquvb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cziyobub.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hnmgavto.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtmhspgg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ysfedexq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kywrxofh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nusqulzc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eantwthc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txxafinh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nuekyqvr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejxatpon.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cihcywvf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3upcdckrk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wryoxovz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3skwwlehq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3htfukypb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twwpcemk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qeqywxes.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3azbnnoye.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gmjrwygg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3lxzpgtpl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3pmadrpcv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3kyidnzyj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zulhxhmk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ukuixcir.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lqsqqcwr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3jcwtdbjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oigfmnnr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qvrgovyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmmfozei.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vvfdowiw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ogwemhsf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xucwaqnu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3amrhhipr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3wzvzddvq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xbolumdf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tlirfswh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fwudholp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtgzpnvj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bllmvmkx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3llmiwqww.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftccbkbl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3icvtukql.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwllzjgp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mgshxccl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rcizlawk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3beevvsgb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3idgyelez.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3opcoibkr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pnhxqbkj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mddywemx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wvjtcnaq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3svqlxqez.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nszcufvd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pprgeknt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hupznhic.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fpmdpyfe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bxvamxtf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3npkfuetr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ctiwdwjk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qynygpwo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckgvsvdv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxmxknhu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3evxbgqqy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bgkvjwet.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pvdupkag.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3hwhalwmv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qzixsfjy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfqcyrnq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rysteclt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ixifooqd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqjspucq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vjgansmu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gpnndyqr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3afdkezdo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3azijtxek.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3qqotmskw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzrmmnhv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgcsglhf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3onzwvytn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pqbeyped.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3orjcecff.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3enhfaynw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wmuwrpbw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3cxqetjza.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3nemctuyo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tozkzeli.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cwkjejya.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3goxziuxd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3przedmpm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3phpelesc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3xsbrkujz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zvyzblzm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3cviqlbmm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wcnudbqd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pehnpuod.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmnpuzav.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3btxitffm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eoyubdof.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jmvugexg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hvxshbxw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xlinuaub.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ybotznrr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3jmzdrkln.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjqacpym.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hghucynl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3plafiihq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rluerwbl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qeceyvgx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3mevcsdyq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewtrbbrg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pbmyhnck.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bzidbsnj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vklepklp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dagrhcos.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xpnxwcid.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ylwfaqvz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oslygxbw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tenhuzvq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3psiczcuv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3fnlhukvi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nqhhpfcj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fknthvia.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ufqlkqom.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsykbujx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xokdrpec.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nppgapug.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yoxpvagk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3tusehpof.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vuigoegw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qqnistqf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zqtkuphd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3byoghzje.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3siyhknps.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaosneas.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wbfujzqt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xjcuaztu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3necftpwq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zriudfzr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dqtkawdf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bmfcpisl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3felhkfxc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cspljfed.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xwnqvfso.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3kzoiulmc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3zwmfnkxs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tqwmtuyo.html


<!-- 参考信息 -->