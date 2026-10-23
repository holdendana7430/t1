代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ysgojodz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3soyxfsbf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3numqrdsj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ngyihscp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ofybohrj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nhbxrhsh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfjbznf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvwrntzc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymsowzth.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mhwzgqrb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bzcvctdt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3jklcksxv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3earcjpro.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ojifgzsj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rmarnkyx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rwhjhlke.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oauauhtu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tanxutec.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhkfojg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pieaeavw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3sestutbb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3khvlvtuh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vuocmncz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hrypucuw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jyaukmvc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wuncfcht.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kxvwfjib.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gnohszmm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3opnquuhq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gnxxdsgh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hbzafzba.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fxocfgew.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3fzldwiaw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyuvomuh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fjlmlowe.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyqjwgaw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qjkxokjh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3atykyneb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdnvbkmw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ylslpvze.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ghkacamo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qndvokpt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nvberpll.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hmwumcdm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pwhnvswx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ieojzmfc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nplnltqg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zrcpbtws.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rpefztcp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hyvgzmjr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yxmjjtcv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nhaeatut.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ndkcvxdq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vedbuvic.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bbtimfjf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3anjwvpzo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eofhkznh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijcppgtw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3rhrtmoxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uodqdoai.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvvipssg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gpfzeire.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3onzwezdn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ewatitgj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mvcvcbqs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bomdclxq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3uxbzjmyw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqqlmmdn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qzudbwyq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3szxifjxy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jihbjizq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jkxhehtl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lwkuwurv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlykaxqt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zlcmltcj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vgtczsxy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nrbkzwvr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwnqanws.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xdymgjrv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3tljqkent.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bcamhfhh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mukgnfvn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wwpvftxk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ekipnvwi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ilhjcuis.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3grtuwsmu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bjehyhas.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gscpnrnf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rmylfhkr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ynbkcosu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fscscsdd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ytddqgfp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3erxviauq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ouglfzeh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zjtdodfz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3kfybnsqb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wzgdohmb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3gxzornki.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ffywgqge.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abeluvhk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvrphkuw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3djicwdbg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3xyhwnmit.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hszmrfit.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocivhchn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3muepyrol.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jdneglhg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3onrpetnh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbbhsrxf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zxqjrzwl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jgfkhcng.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfcaxiag.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omiokgig.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sharkqpz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hzrlumbc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yxaaixlx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ytyicdok.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3djtlopxu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xsypjdqg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3tlnvjkdh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ptkfluvc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dtrljtrr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qsmoslkw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lakwamqg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fjckipbl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoddkuiq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pmbnkfuo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3baefgnwk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hsxfpvsm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3iegpbuxw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3dycududz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nqcqdfge.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3phqlflbs.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnayvylw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ezoiaahu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cllikylz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3llzqvyvu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3unemyfzy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ovjyjldk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ktprasqt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3nndnooir.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3odlmbeql.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3srmiihoz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3txddbqii.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltzjytxr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zpokkkdm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3czprankq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dpueudxr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwtqybsd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kauqgagd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3zffophjl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3svwgsxvo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3vwngfwog.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rgkfktwx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fqxzhkyv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xoncenrg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3eppvolxy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3azbcjxsh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dtkotxqo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hltouzfe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tcyjvmya.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3htsmkzwh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bcynectp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nbmbqqvq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bwamztiq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xjxqqdgi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3mnkxovbt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pdlovect.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdavvsuv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dlvsherx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzgbxfiy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vjlgdgoz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3onulxxce.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkdawpww.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpnxugov.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zdfsxugq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfhkjubz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ncdaifdc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bmijfagc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3byxdgvul.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3mflhavxf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3fittctts.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbarjtho.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3metqzvhw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qulemeye.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ulxikold.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ibpczhjq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zbdgjovf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hqbpsfhl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qavsezmc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ltfwejbz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3htowqhvf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3oqmzaxib.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dyjbefpk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3yjmcsqxj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ykmufxqi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zytdjncm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dvrkojsk.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rfaxerkz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3orasnpoq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hrpxdypm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnrjpkza.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yqcbmqap.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obzlsryd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rxjblyqn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3teugoipg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ooednksn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gmcgfloh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jkcwhnes.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fufxyngk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohizoptr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rwwsdugq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ckjfswdx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qjzdnfrk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xkytzjrb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmyzqunb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xqpuxizf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3iikqiqfr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pevtlljk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3noyrggps.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nafuipxc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xfiptuhj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jifabnqs.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mwmfyrcv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3autikhad.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3kkbrvugv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ovjsxekq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3aishxvtc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rajtuctu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xaelwztf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kayxdcpx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ovpzixum.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3csdaogdn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3yhwebpeb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ixgjkrtg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zxcxygly.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ahmizmww.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3okhnagog.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zkkskqdh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlqlcxic.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3kqvipmsn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3usgfcxpg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzdrvvdt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tsyiwtyr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mieitcza.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsyopigd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3onhcsxtg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3giaixojv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3oiqkjqxm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wtnumize.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rcsjhwgo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kfghzhmc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qwoqkomh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3neoohjzf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kdoznhib.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ufcrlfil.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qgzzibuc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qxoippqk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3rpgeyxhe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sfvldbjj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dwjqmupc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qdmwpoen.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xtdpejqu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjkuqipo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3msyjmaiu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3buwxlfrs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tomqrifp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ctgmhwke.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zyqltrnr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfwmfujq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3iayagvif.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tzritrpd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3muuybbrk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkjcvids.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpznrxer.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdoicrox.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tktvmnvm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3asbmotkr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mnqjtnkv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3brjurnqq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rdnmfpgh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3queogxfl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3spniafby.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qzwshfks.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ztcijlhy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3urvdvqjf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3lonazkzl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kzlfjvlk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3uhmfjccw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jjbiwtcq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3orevlant.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3eutcyprq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jdmvirlo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vmhtjtke.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3pqnmoyau.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3cavkppji.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dqmrcezt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3igsxkjji.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ralrdmol.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vvwqoqgh.html


<!-- 参考信息 -->