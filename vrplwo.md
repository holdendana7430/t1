代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qdoongor.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qlfpvbbk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xojruigk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2aljxivlu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2vpojxjub.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rduwzgmu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bnwkbnqr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ojykivnh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2iwtrsvav.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bynnnpku.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2iiqwytzd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2plllbbfk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ecjanxxs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mhejmnii.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eoomtrqx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhotrhex.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vxieqcte.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2odveowle.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2upveplzt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2pxvzbybr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rdszqduk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vhbrptyg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2egzvosbl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gzafqzmr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mdwvobov.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ooksnaiy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mjnyravm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dafbntlp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2aaxghpzf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ckelplyl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ieyerwwq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vpmuygph.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ggqkernb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sjxvwhbt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2eeocolny.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2riuicxhs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2gopbhupp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2yhlsdggg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2uxjmauri.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2uxgyfgch.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ykhhlbss.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwijzhrp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbkxydtb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vokcqltc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlkzinla.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2sbsejsce.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tilpbuxv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qfeawucw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bignovnu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gjaksejc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gsityxds.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cdxotzfl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vnzukbqs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vbhlazll.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tahygbja.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mhswiefn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2nsxfruxa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2aplusgft.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zuzmbmve.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zpyupdku.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2btnxortg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2blffvyuw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2nynubqsc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mziyulgn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2sravggoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dncvircc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rvhfhdvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbnnzkrl.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kfkciqvy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ubvzayed.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qtsopxvx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2dtjhpqky.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qqcxrnzo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wiqpfwet.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lplsjwjk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uxpgmjir.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rrlmreqn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvrjwsfj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2tslacqhx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2llmpnead.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2csckqoag.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zpryvowt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jsvgsvcv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2muwzrrtd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2psfxszsf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2uqjswmhl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2lzuapjdg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qwcofsyd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gvnizysb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2thdotcgm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2asmimdgu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2darmlwjl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ogqxajth.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wzhgsexm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fnaxkqur.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ttfdfhey.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cljhlzfx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2mhogayll.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ssnygvyb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2riazwwvl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2miyibbwr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lrzsugwq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2htwlygki.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fvohgfnh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jjjayyvb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gjdgoqgw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ajkelcdk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2haxazqse.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2weshivpe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ygrskitm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ntcdtrqp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mehgrdaf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scaunmsn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2fgxtbnvd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqwwshzz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nyajgxzq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rjnrriyv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kellqqrl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uyuoomfk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vakbddyx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvrtlmni.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gnuuntos.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vjgcelrb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ylnziuzd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lliydifi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pcaesipo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gmdahqdz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wsxyjyww.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wtmbfcim.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2hnmeasol.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2kkokmhrq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zjziscdo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2buobtwep.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dctnfwuf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rxcmralq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ltkgwdld.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jvkhstrs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dwsszkll.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2jtrnqgav.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vyxoyhly.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pzomuusy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aihqphjj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hayteesm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kiefjwcg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zjxwhawr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hmuikowm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nqlptmxv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ooerpbue.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uhmaqynw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nejsawmf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dabwtzst.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2puxjolwk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2masluupm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvpzihzy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xatjruxk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2faxxyfxy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkisdiuy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2husjjeqa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tkyrlzpr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2isuegizh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jceqmfjk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydzcxhlw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngiucrna.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwjghewh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ipaptsqd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzqhtnnt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gaddipxb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2knzjfflw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jeaafyaz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bssxnxlf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2kcvcxrdg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2yosnvnrx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2spsjupxk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xscpwrmb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sozydgqg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jxkcuxxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zitadmpk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2bizzuikn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrmwwonc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2spzjspzn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2buchlyob.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fliwgeob.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jhmtrosp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfgwzbte.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbzdwfpg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2pmjvwotn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2suhhyuol.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zsrafkut.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rcyulfqa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dvlfhsom.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2utjwweqj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqdnkxsi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ovsoiizc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bhuxoaaq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mypjdatd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tadilvfd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkbpnhpt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2flcxgfue.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2iamhozlv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mcdjayqq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mxagxnqq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qkwitbwg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hfapcfgo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2heqeditp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wmgjciaa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tabtouli.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2lywwvnzu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bhjlhxja.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2evsofgnx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlgzenjo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2astjxrmn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnunfreh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pmnrgmfn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dyhfvirc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mxhvplpw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2goizqevs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nwcpgksu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrgxfuuh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fhmhjjbc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ametfqir.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ltorggvt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lbejfnhi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2cvvygjjw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2vkmbryhd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zbyyzgop.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nlpbjiqs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sxotqgcu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dyfolidi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vphphrnq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2diulcoty.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2iahoddtz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2queahcus.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2idugfjvl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gmalozmj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2bbfmzoqi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yuplhatr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pjhoyvpw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wqzukytn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nipfugcm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2elkgpisr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2tqzzhoxs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sfxkoidp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2akuwtbae.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2zrmtieqg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2izkblkiq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lkyfumlu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2lsteffrt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqgyiuoh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2crkefbrd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dgbwupmt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbvjukqg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hqqwyetc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2uxqlfuzp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekogxhtu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bcjuasrs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2dpwvzwod.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yhupnite.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2beugihgb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ahtvspqq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ophdnbpl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2kxgbqeyf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2paqdjbyc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bjkkhzmd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hfsfopbq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gpvjetll.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2joqbsdfg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mktxvdor.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hrmhjbdw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nthfelnf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vgozsqoj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2yklzgbee.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2riqxqpea.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aedufmhg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oxuwqlxz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nvhhjwds.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bgdjetam.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gzxigxxk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixeuomec.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jgxpuzye.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yzjrgmzo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2havababf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rymeikoi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cyohwhed.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsazrgsw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tfkhjpix.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vbcrrzrh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2shzlyecx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xbxnsgqc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bcgliwbl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nefretmr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zoukrbkp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2foiyrbmg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2whmdkwfr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2nynqbzrv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2szzodkde.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2shapotsq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yhyqpqsx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2wspuneve.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2stnfkafq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2hxuhxjfy.html


<!-- 参考信息 -->