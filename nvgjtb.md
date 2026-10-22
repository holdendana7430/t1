代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2izyifvos.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2uwunimqw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qplipdhx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ftjppkvg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gceacnfv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vhbnxkgp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tryggzmv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ahppxxzm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2bwrziznf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jfssldfz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jesvnrbv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nskgudux.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2iemccekb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ckgiczlh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2upbkcosk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2iboituds.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivawyccx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zgmygqag.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nnuzaxnx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2pxmowxlt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2uqyonkmf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2kjilggkc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mnsznwjv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yzsmveza.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dzpdcife.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cdcyhjuf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2clfkljnn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2offnljmu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gchmezqh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ssevjsum.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wfwpxhho.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gsvlhgpq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2giqdlrjn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ixmgfrhx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yhdzqedt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2aaialtby.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ewaaclix.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qyccdhkb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2hohflaoa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2pbgdhjuz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nquobuqc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqiyowzd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfpzfutq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2geggsime.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xviqcagg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2gsuadgrg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjkiwfya.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jujloadh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ghvhocoj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lolfacgt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yipezafe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wixcqhug.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kgfafsms.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xlsmqczp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2abbtsgwd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2avtpjxgk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rroogxtu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jolojqek.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zoytsnru.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tiqttdqt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kaqkepnt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fqtxmher.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2sugmmzuw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2icoqlcok.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2culywyry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhxavvnv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dlfmgzcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hctwntrs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bqgdinhe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tzotufvi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szgsfdxn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2cfcsxezr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pmeogast.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2murluccd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fubxjdna.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ohjpidku.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ocelysef.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zphjczcr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2riebogxe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2iavehanv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ieotiyya.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxjmabhc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kvoadklj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2okeeqozr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ezvfhunn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlwvmnow.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vbyzzvvt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zzdaxfle.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iululdlw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ujpalbdh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bmojcrbn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2iohhwipk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xhlujbxo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xpzdogmn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pzztbwzr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gbkshfvj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sfugtadf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2mchhfxgg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2aeftinvn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pvnstlal.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wneewywe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rvociirs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2eridtzha.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sesfxbsj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2frseietj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vhgthonn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jbpgxxzx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wplclyro.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2agffuctt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kxklzwts.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wvrtzldp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ocgzzxnv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmodimkf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nvqpjuma.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nsoiytwg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vjrgklrq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bghkmqgd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfgomaim.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xycjjmtt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bavakerz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxbxksvu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ywbvrxcg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bqkpmiyu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2odmjzzlv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2axbrfmlm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2umhanvbn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gjveegqr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2twspciin.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwokzym.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ozkzyfeb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2atzmqalb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2tslthkrq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mvefbtza.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2udihynbb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gguzoaqo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ehsiojtu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qfaagdpv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2izxnkqit.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2mhgusxlx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ykumtrtj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2cklxglhx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqebuimk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ggzglxki.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sbehyxwy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kxwokfpu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gwwydmua.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hkinvykd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzxeqpmr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2osdwdyeh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ruooktwy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2knmbbyti.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2icvlamgc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltqimneg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwwbumqg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2zoeqgmtj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldeboahg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smcjlzym.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfjhjsld.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jvctardn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xpbznsvc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uksmnotv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lyvuzovg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2prnxwvsw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2afagwfrb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2trpubtkv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oidcfkvw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qfalonho.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xsxaqzpf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vnsgfkmn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tmxpbarm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2scassjqd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pyxsyyje.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2uzlhnazu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2oyiwrryj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2flyspslr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tzfgjcqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldunlxty.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2eqqijjrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvfxungt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2fqcdlxiu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zoqlyrlk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppmkxzli.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2plxcdkcj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckibhzrg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogojbmoh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jrafxcdl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rgumqpti.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yqvfrkde.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kkxnxtoa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wionthpp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vcwjebjs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dquckrmo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyfzjbdd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhazqyjk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2uuamibqe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2bvbevkzb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aefaphzg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qnpfuhjj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ghjymhli.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2eoveabnp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2drljipwm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2usjvolyf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2iikdjojj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2djfytury.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ugmvpeei.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dcgnhhig.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dgqjfumf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yswlbaaa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rbppuope.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucqtknvy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2muefcvhe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueqdwfqp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tzaygodd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gobodeay.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tyoepcfl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2gmpiswgy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2napnapou.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fqhqpjlb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kuwpkgcx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wrcctzwi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2puxwpkpa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2orabjhxv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2axcbjhec.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2nzjcgyio.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wafiqwic.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2fyzsqvnc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkottljb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehakldye.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkivxlba.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uffojnox.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2muslzlmo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2fpemezom.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zphhjsrt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wceslurv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2faarzrcl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gthhnhco.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ijptzlwp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2chljdooo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dhczmpxe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fywpzhla.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2sfxzyubu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qdjengil.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2frtrthvn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jniktiip.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsfvtfkb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2haevyjzs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qekwxopz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2uifaeiyw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jbpkngke.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qzjacwxq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2gzrqaemk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fyyehics.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ynpkvwrd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnkgtrov.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2yhmybvxd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylckntnu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qypcitzz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2pwnzfvhp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2eihpqtwh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2knomvhci.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2crtpbobp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ypxjcwdc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rcdrrssc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2sksgrtiw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2leyoebfv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wmaftvcr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2djnjdhgb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kazgrzqd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2lesocqbf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bprtvfdw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vrkrlefk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hofpdvlg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhqgazhz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qkkqnzat.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2npxbbcpw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mmgkbqmj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wwalyhyl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftkxatqe.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yazpziay.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2beepitsa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xktfpanj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxvxekez.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofwauzof.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcwdchul.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xidpipho.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gxvsosfu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zoipnyir.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qakmcbgy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rhdrumrl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ugwqpycg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qtecferu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cvynilkt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2irodfbet.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2voknihom.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2olpwmkwe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gnvpaeqo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kgobjebc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2fhvrbded.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2sxrncnyl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ogxfrsvs.html


<!-- 参考信息 -->