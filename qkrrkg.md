代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lxoldzew.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oaonpnwh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fuxnctbk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2udwzaesy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2impgjwmu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uorhwakb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zwbjkqxn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gxsaaugw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jvzjslze.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zhmkjegq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2slhdxqcg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fdbiucyq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2tvxkrfcy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hvvsflea.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2phbhjsbc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nsuaijrl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zqijsiyy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zqrhkads.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tpetmaoo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yzlkzdlx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ymcrgwje.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2gfaaewky.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2eabrmnja.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gwbeyucg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rrmfqjdd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gciqldyo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fqmjjdtb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sssbxrjb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vqaqusct.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2bnxuxkaj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lekhljgc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2tevosokr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hkdznffd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kzlsgrwk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgieptrl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvlqzklx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2tifukvtr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ukxawflf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eckkmcik.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2payssubr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2brmqawjj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wceseuup.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hwozmora.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bvebdcan.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mjcfzzcl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2yrunzizz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ohsxubbu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oiprkplg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zoxmgmjm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lpyounzr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kglwivtk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2naxfracm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tajtzfrx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ffgxecps.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jwgujqnl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mevjhjbh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dusogdwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cetapxrh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mzoebecz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqcrrlis.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mjxaydak.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2glxkgfls.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jyfjzldr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2mzvniend.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nppqjruo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zzmytqhd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vxigwwpx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2svbckegu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bxrmquaa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fhcdhjqx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cyxnrrvr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkvuznjx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2oiokzhui.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgbjvhlp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pdkvlkjs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2hybeyarx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rjamdnra.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fmpyhyxa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2zlnjxvjd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jruemour.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xcmrfcem.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lerqqzxn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jffyuczw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mtngigyd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ukgtwwlp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pafsusuo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vpfatbcr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xlxkydaq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zkvlbhmu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jugveftp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qpemqzyz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wqwghivz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2jkyqnpev.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nujbjxha.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fxphgnxy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dtzgspyy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tgxbvzue.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2irmewwtr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wtmxinww.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixznkeou.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdzamioa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ubrimqrq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2yfdfzyln.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2giuynfpt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2udrodnoq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2daebskmj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jivtcjgl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2khpdplvp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wibdoclx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcqhrrno.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ecbvrild.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhxrrmwn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxfkpqhs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jiytzjbh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ggpsplpu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uharshda.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iyunfpnf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wbkvrcia.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zppytqeu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yfzqqqjg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2htkgxzsr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2miqjbzwd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wqciaqpf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2quixsbgk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2trtiiubl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hqtdllnu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vardfxfu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mkzweaun.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2scgwtqcp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fwwytivz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2limfnyhn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jrdjwaaq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wpsebngk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwwgkghn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wxungqig.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mmigkjly.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mouawnvl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jsrgdowc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lqtwpwnf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgynqdmo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2gvjxmptg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2yrtfiojl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhomnkat.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ijarbxga.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzczdljt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zblubfgp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fmubgnru.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tyccbsil.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxexqxkb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqzoqmrn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xocguckn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvdkgpps.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xqcavkub.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bxhnohuj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qefbnjkv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2czqhqtmv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2efduptua.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ffrittog.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ppdfgjwa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2idaknlxg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2keizfucx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rifmbhkg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dkjsfabh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2sftnkeeb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ctdhvdyn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2popxmhzj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2amuixcdh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2cujemhdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvixhsor.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2obxhvjpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obcblmlp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2jouhaape.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2paarbhwo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2tgnanfna.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pnmhfwin.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2saxwidua.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mddpkwqv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2givydjud.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2naymmlkr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtzigvko.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rkiqdusa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2shbotntf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2plhvzkrt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lqfvztdq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qajmwkcb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuemspuz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ocsbecib.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tronlblw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzfaocdy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2oncglgvk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xuchwlbg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yxpeiudk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wavwfapj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wgiqpucc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nfnlgjae.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gjdovyxa.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ahrxdjub.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2aqktfyda.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kvbkmtih.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eoujlpvs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vdkwfehd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rnccewly.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gurynsrq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fbvrgmqt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zlnkuizx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rmlsnbkz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fjterecn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2oeqazbch.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tsnpahsf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ubwjocsr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zltbwida.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkjufjej.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbwhwfxp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vvulgjtq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2uzdkxosl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgukxlfo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gmwbtjxy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2njobyoxu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fuqfyncl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kidvsmnh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyepfjky.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bcokbclv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2eshormxb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rjdkuwdc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sthztqep.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nopiudnl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2fisaycuh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ytcifhrc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kuylipxw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kmbhbthq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2khakqqwk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rcxfhxjn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2sqiwacli.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wrpcplfm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wqxwqxpc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ppqcvykw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvktppcc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyzpsext.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dvfzyaqj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2wcqgghua.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hmpeluxc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fpqkzxvl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cshpchcj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2tinlvbnt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ipjlvwsv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcfnlyjj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qkrossvu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaviholc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmemrbqm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2pdnzgbqi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ltfvixkf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfwihmqy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vfccixns.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zhgvtuce.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rgogldgg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2tzaryjsp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ecruhmst.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nwgutnwt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2hkxbfxju.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ncwpfeer.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hljdrigf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2gjmtkrxg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ohleheqc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2thpoebzw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xmuvyfoq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnbthcro.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ouvrjzfz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fnyaifzh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hnewooww.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqpbhhfc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2mbrscnua.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2aznkoapi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ryubhuxs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ufbqoijt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bzmxnwte.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2thablher.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yhmpxjzj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lmaldpcw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pstektrj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vnfhayyh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ukjhrurk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pjplfrox.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fjeesgpl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qaijayuq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tqxpzlma.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vuyrtojq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2exiovvwq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2oscvrdhg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kocycwbu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dwdulkkc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2mxoxshyu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xoofcttq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pujmszbp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiylxfjm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fsydveen.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2urqritve.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2brzfrsyw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vyxqxosj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2leniipph.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gqmorhll.html


<!-- 参考信息 -->