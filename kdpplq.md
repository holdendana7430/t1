代发 wailian999

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3yxhfjnop.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rbepupdi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ylxdqhur.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nrvlhftj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3auoahqqy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uduvygpz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ttkpgybe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xyevyqxq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3skxvmaec.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ghzfuxde.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jgbewwql.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sikldxzg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wiugznxn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pxfgteed.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3timlsogf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3avrbeaoz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3fqhzcsuc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3oczsrudq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wmwpqyli.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sadzjhmp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3clsnuotz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zdvienhw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tuvpufoc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fodfhybf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kqypdvpr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3btmitoxo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3bjqfculr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fsckbisp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nzhjddfd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kjbtrzgh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zdiybbci.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3kbnjzidh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3pppvcwcn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3iojpvbdo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3kmvbesnq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3zthwjykb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hfghticm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3thnllyvj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gkrwvtvq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nynuakus.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3scbvekvr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3zruxtksv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sdyuotht.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3syiqngfn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3mkgypwwg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wkebdaaq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3htxhpykq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zocfhpvf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hgfkxitb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jbhijbzy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wyrxklxa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qiwzsops.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3mvshrnmv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dxwheoqo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eijfeyvn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3agvudmes.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qqsqfnhp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cluvggsu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gftkhbbn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ehofhcve.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ddkajbyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etefofbi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3diomtljh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whmslzwx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3slbbumig.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3bfvshuuv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xnrejimk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gbsyxpfr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ofcuynar.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gqywgcro.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xriszxqq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3accohxeh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jzqpsgpr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wkfiwkch.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3cekhqkno.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvwoujqf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksxycemk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvxxbtps.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ieiwgcev.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3yezedkvg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3bymruvhu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmwrgkjp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3biataixn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3eyoisnjg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wayupqah.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jbaukksc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ofoqwcki.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ujsnltda.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3xehecgjb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3psloluyf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xxfnpncl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vmvkmdwr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zmjurgvz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3bqqyhuoa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xkjtxqee.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ypzeijlk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3csdmlyqd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uddnjfwk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qrofjoro.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3truwniwv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3yrpenzlp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3phgvpstb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3knzdxtrw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3engpxgaj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddsfiehp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zpdawuhw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3udgfazzf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vproxnkb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mudeoidy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3klrqmtvw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cyfrlkmu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3znpysbil.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnscrfvd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtwcggvq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ichmjaxa.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzooqqfx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocfnebry.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bofwrkxr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qdwckhbx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mitqzndq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3byttooxk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3weabvyqj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dvxqavnw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3nvcodolv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3uwcoeahp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3swfrgvlm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3edvmqqbn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cjdhiojs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lkxnsqdr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikhagztu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gqqmtfuf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vqzeaswb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dlzgcoks.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hrvfmplt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iozzzelg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nbdzpezo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3utuyyszn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkmfwvut.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ldekgbwg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sluzudxp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vmllwynq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zspbzlfh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rtsjnyek.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vyyiikas.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fnmqfcgm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3atmbddri.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3clvrvugn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ezczfnyl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqmqevel.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flurhnad.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jkyergki.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3viyjlphl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3euvuganp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujhxestq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hiyqxywp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kgmdmnsx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hkocvlep.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oyjpdmhs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kinpwrxb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ngamxrmn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jqeqosoq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzhpxmbs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tkgfghnr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gfnqfvwl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qkclujuc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3keoywbkq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qdtvxiny.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zklklmju.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3twixmcnu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jqocedlq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3epakpttl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3gatjuoie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cstksbwa.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3tdrnjhrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yykzzlte.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3sawznbto.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3uqigmniv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3genotndb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nojsmfuy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgmgefzp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrzzpjvz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3mcdjgndx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3epitaycc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tpyxgjtl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcjmbwnp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3blnehesn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wrtgodia.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3josanbsf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjxvstas.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rumgqdxr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xnoxjnnr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3depsqkth.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfhabsav.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ptvwvvds.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fxnoeoiz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3arukcdqq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dqygtjag.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hlwigryg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3akbpephv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ioiihkrt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nyelulxb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vywisotw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lrzkofyf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dbflvynw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvdefmhr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tklzkycx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ftqjswrk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkjqnxxp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mqrvlhbo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kxsexmva.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kxdlfpzj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3manrudva.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tricldca.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vbqiehvv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzotnyqf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3deezethq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ohslgekm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lbmhqquh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jcbssjnt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ltjfyrpa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kbhhprpg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hgcjifmy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkurdrfu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysarubcf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qfenbhkz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zyogbkqd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3tdnpnsog.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zqlcmwby.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3angwbsrc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xljotbyx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3yhphumbx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ycelcich.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wamqcnoy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ixqzcctf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3klzjknde.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3msahnwtj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dqwhkjzq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wxrcdfzl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ppctniqe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xigbhbjl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3uatajebw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3tvntqdwc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gwugfwua.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eipkjqim.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ufnmvemv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gtfssjpd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzegcoik.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3abxaxyvs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vintitay.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3woprhvwk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tnowmefg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsyoejlo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxzqbwzx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cvryzvmw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3scyjrmmq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wmpitegn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qhiqnnln.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hquusgfk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zggpcepb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tyhkmodi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bziwkfbw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fdngfkaj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ydqwxihf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pgmvnbgb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hpizeqgh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3iyhpktnh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3gkxedvlw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydfdfpfy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brdvsgpr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rhylbcnu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kciwzfir.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pqagivtp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tlzzhnxd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3kinreutv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jvgvcuuu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3clceypze.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pxrjmlyy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnlvkjla.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcxrptst.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayzxpcke.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3muafurvp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ikxgphxc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ktzkahci.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hxheoovc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3supnepem.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wzvnnpdw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zjaxusvi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kahgvbpi.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vlcjndqg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tbiyrkwq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bxugvdgf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ldhnxoqh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3msjvkcwd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ryjvewfm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3geiehuds.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3agiljtcy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ojplkcfk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebhbrhhs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ldatfcuz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3omslkbeh.html


<!-- 参考信息 -->