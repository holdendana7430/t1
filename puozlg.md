代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2psuvnhvc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jabxqane.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zhtfimct.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ypniucry.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wwpzzavk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbeocgoq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lhuaitoh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2owmqzjvt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ilyrxbpa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ddtxxgig.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xyafkzxp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mdgnsszb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lmnllmtm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ysxdyrji.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zobipdaf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rwiijaha.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rykehwzz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qucvchcn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qbiswwhm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2eeojamdc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2daeykzfu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2kkqlwqby.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rsffegwg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2faukpmso.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2vofwhtjt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2iuioqrbp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gnyrkpvq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ssbvmjmt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yqchxjws.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iywozpyr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fjhbzvof.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yemedxek.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2olqctsyd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kndwnylz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2bqtxgclb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wdndbzhk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jpdfbmxb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bugnfslt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rinqksjm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gwnpgbzx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2tsqgequd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2hhinowhp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2zjidsibs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2akwueydu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vuyvkagd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2aijpbune.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdkjsmrg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmrynerz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikbaqwrq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ymjsmuam.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uknleluy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bjnzpaov.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gmkrkors.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2djhvqnmq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sxyficid.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2luuxuvto.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zclhpjtz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ogjqlmfi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2epoybtgu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hbhodfms.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2clqeclro.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2rywlsqup.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kjqmmfhy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kpakewsj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tjmtxbje.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gkugzgrw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ulnincgp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rmrlawsu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jovogtmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjuctmfh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2obmkhcgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyyaoegt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrkqjspj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2eolezzmb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wqoinshp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nnhzyroc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2usdpdsmw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lzjkmxhh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mwcyolex.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2asxcohhv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nrdhbezz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2acyqmajo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ivafejhw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2yovbaihh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ovylqbro.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkhbetui.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ziyjbgnl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qzmzcgrr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ijskjymk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ftjlgnpm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kvryxfkz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2nxnnllgb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qxjxbzwl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2twpbapoq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mbsarvvd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2clkrvxox.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2uyagygzg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2nhozvomt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cuhhlkju.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2sclnacqc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2necjqwkx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2iimucaxq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hjlvkxor.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2aejqxsox.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zeukokut.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vrjchfpo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2pniazfoy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jzdqrkhc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rsakcpvc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qtuopgtj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2alpxsznf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kivledih.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhopkpgd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aujqufya.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xztbvrta.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2narkgokr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utojlbtw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wffbpyrc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mrvhkbdh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2seyadnnw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asbnbikk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdoyeuct.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2phjfcfce.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgzypvjp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pfvfsegl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tjebsjar.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vfgrvhso.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pkcgydtu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tmdvrwpb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mmragcnf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ohhrtzqr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2tdqasqnh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2lsvdigte.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dimzmzhn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2fhlasddo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2hvnybwxl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2yutgcpdg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ubknokze.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jeermoxu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xwzkowtu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2upkioofo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mkbinvoy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fjqprunz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2sfqarbbe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kkddjhxa.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hgypaezp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xdvejfve.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2roltsnmt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2caiozqjr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cxtematf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lbomjvvh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzmjgmmr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mxvhscjz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ozdlazcq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zvybfkiz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kdugaepf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvddimbq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ttoxftdq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2usadkipd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifnnofxp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmtcwxrm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajifwpbj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gjbefger.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2spexgpza.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2djdaogla.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jltgelrh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcgtytkc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kfpftzww.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2perybznj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mibzymmb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mkqyvgyf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2kxnrpnru.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gnliopay.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2kwyuubla.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2czpksqka.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rwchwtfk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2tneddbtf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pbfjwsyz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rpufifak.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2znzcoutv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhhqaeok.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gmzmztub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fimujbtq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2grlsqdou.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dvdowfqb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xfysmcws.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfxshfii.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ftrgxcjo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2urjygxrl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ghehzmle.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2loiymliv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhwhtopk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dmbioefo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2uzevflkg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lkznkdbs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmrvincl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyybigju.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mzopwhga.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2emowowfl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dxiiukxp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ytaxctxh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wwinhtjm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zpngfoku.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2phzeihnn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kdkxklti.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mrwhcvmv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2gqlbcadh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xvrwxewq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2goovijlb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gqlvjstv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jgfrcjbb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yyrpdyvm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vmodujbh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcvrmeuv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yivhjexi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqwxldhg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zsnarcdc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bhkgrsdz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2njofsvlx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2otkdizxs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2gdyfudnu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kencrwez.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wwmlgwpz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngztping.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sigsyzvi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2dvhdbzrt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ltzzmlzm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jhadyftb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ffkqeuvd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cflumuoa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqqauiup.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sifzcrmn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhcpcifm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2efhkftrb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xaghduos.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rpqtozwz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2cytybqoq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2gmmnehue.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2plmscwaf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2krmiqurn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2efxksjly.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pdzfgmmk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2demustfk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2uhinuemc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2uefjflot.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ahyhaorf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wifcscti.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hxqgfmvp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zjlknvdg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bsfmgrym.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tmbixgtu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukflpyyl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qotaauld.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xgasqzwo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xkmbxgnt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jnzpoptn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kwbagthe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ztthfuze.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2tjozvanb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2yzcnmwxa.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwohqzoz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2aycrvpsv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vvwneqfu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lcuopyia.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2kgxxaegy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2owebanqh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bjyvbqif.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dtvdbgzh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bgonthie.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2sooohxha.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lrxnhdpf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nhfjxihe.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2azmunuof.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mlnltkqy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2yrmrhqae.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qejifjpu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bslzapwv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmswmtgc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uknyorxl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lpxpvhbh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2uaohpedc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohprkxbw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vxyptqax.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2oulbusfj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuhtsevt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcckcloq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vhjkzaqd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeucahnx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2polufdzy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jtufbnar.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kprhuvpk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bpdgjnoy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2crfevwpr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gzwoupwd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2barxtfra.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vzzcphrc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rmvfxfaz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tciqnzlk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2enhfkusg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bpfbzkpz.html


<!-- 参考信息 -->