代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkgycdjn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3bwmrfidh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ybtukegv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yvffdwyc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3fhgcvyzj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rgpbfjpg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lmmxjixy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qkolcrbr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xvojgijq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zvjkbxub.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sbjywzwl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ylvhdnmn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vmwteymu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3bmodmuzt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gsohbagp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yhtbltdb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3indfmqhj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dcberxru.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gaxomzjh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3fyulyiat.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3gkjmsqvm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3csqcoytl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3mnxqxdqk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jkxdqgwg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ogyxcsuy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gctmroza.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jjshvihx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xtjvretu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3oaqotsgz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ewrqvfmz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rehrbgto.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xezfiejp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fejszvms.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uttthbms.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3mwbbabuc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xpwqadhv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ovusztxe.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3rbqelqwx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qdrmyfls.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lcxdwqmp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jhujpnwz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyqhycuh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3oewdqslb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nudatyky.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljomnimq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zyajvnjn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3czjcbceo.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3tkklhjwi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lweajztj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tgnobgpe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iaszxcez.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ziznejxn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3csviaqyr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hqpfnwdf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3brheovnn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iobrifrc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nhshyetp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pilrijlm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pwkcdnlp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rnlfsbbj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jwugghyj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3snnxqkws.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hrwfdcss.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mjnxqxte.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xwfbqxrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oasmgyiw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3jseojppv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydktwdls.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kxknlpjv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hsapjoqa.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wimrhezk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zmaldjoz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kjbjtwix.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gcawvdsn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3sfveddwh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3prukbjpe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xiqrwkcv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qoomalph.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pztkhpxn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vdulzjtn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnxqjdri.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wakennzl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tucpjphi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3fvqidprh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zuqxjskk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vvyizjum.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3gisxvwyi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3sbbnwzfm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xazugzdx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xxxybspc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3csgpnnur.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ntejxcme.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cghrruoc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qmqbogtr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lyaivcce.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3gjsqadik.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mxnexxzs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bvbgzskk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lgjqkekg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mmxfgzhv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3flxfpfql.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3likkyeer.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3usrdpplw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nvspvvgz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vyujninc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ocligyis.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qepeqzup.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ioqpufqb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjogpoeh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3egctqoqf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yechufkv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwbqulfo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhccwmnc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3smevlmji.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqfprwpv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nohwpxyn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvxhszwv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3myapglao.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yufvrtfu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3focjuwmp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntidxedr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rbhcrrws.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3okqzntlq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3teggwxiz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tnioqeab.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zvdggkwd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rkkhfzxe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3efkgtbsu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lyhkqtbc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xvdzmilq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3eryhfwqq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3yemqpvbc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qdcnltpe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrpgsyiy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jgiidtlr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3runwmzdg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwboklz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jqtbqgaq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dddgozct.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bkuidjlh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hjitbtgr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3omamgaei.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fqqpkfew.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xoaonksg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hrhqmxok.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aqgkgvhc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3dllhftbr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3malkyvev.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xxkhcaef.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ghfkctub.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxekqgyo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sjkjlwpp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lizzzgqj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ienmsoad.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kedmcwwi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qcnzagcd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3usuddkvy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aaeipfkh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3osfktxoa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxtyqoji.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ihgdydon.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ciuugsjz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ymusbeek.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qdxpikez.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jujgyxkt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pogqojsm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ytuvbotf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3skjzvewf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ckvrogmc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kqcycknm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kociqhmf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jwdphuag.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cgymtuby.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jjybcmau.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wzizigpn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wpupadca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcpwtzwf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ybbfgnhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkzmlgbr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lnfmqouc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3itdhxjrr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xgmrczal.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvfqsfdt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3pzopbiol.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3kepeuamd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qxkkhpmf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fdbinrpz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iafxozno.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ryqvklji.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3bytufusw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hrugygth.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxnqqrgt.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvvcznpr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fvrvooin.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mrbhqvsb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kcuitcyi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cgawbbvs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3xbcniqcy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gllipytx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3spckhoru.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vkfpcgxz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zplzlqit.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qqxhqvtf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bydtjizh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mullcrad.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nvjyatjf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3eavslhze.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mmyjznrv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjebvtot.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sxafkpzx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3amhtehti.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3whggzffq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bctqbris.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lratemiq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jaqkeoki.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3hdbplean.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rbixszxq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cvagzsvb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cxhzkqdb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3usdgjepg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gckmupzy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gdkeeuak.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3syxqwnox.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtyotovw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rhpdfdcd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hdfyovwu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aqipyrhg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jklrhcef.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkfvpzlp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ijcdpqnt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lckmrdyd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ziegqmzk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qnfaioex.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3hsgvlspy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3clhqwgmp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gorbdlpw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oqbihiuz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xwtjprfo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lazajksb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vuaziiwh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zooothfe.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xgssujhx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fyqndfsh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wpebexhc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3twbbvkxx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrmgrvid.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3fvnojcfc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nowrturf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ixysczil.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3iqugnrlp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3liznkusg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3huvgxqov.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vpbqtifa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zjfskaed.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3quqseuid.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3nrjyduds.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ilfrkkau.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rvvmlpdl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ghbuxggk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3zkkeyrtg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3hkwgiryl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3tbfawkle.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fkjqgpgu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mylxcbwl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ybmvijhk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3irtyjswf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lcpitaen.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dsmvaomx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vmurrfny.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3crlallxi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xbadllzz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbrozccy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqainryd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyhllprf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sctyxzck.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3asyhacsl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3izttsman.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmznmvmb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3owvtwufc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wbfvhpsd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmtjzlcw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3whibnrvp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ihhmjvpn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3npgwyljy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pxlxzcbv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vxbqdubi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vfablmme.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3usdbexls.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3cvnoajlt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kimhdusq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xdhdsaft.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uwpijryc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jitzyvgz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3gsexbphr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ztuidbqn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3igbelifr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rxrebxfw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3jfazuuyb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3mhsspdlm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3scjzrlhm.html


<!-- 参考信息 -->