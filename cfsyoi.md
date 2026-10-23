代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kooxeigl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3srvefllx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nmkyerwy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzysgvlj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gxzsttdp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ylixxzuk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nwhxicfq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3awdoyczw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ayolfogz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wzgzuart.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3thadoiln.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sdnabuvz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kasmhwir.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oqmhioia.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sgewddjs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tphtjslw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hhubmsuc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3khmfmqrq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3afmfrcbk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kwzsovfo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3onudwutw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3acqztoks.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hqriiuka.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ublwgcyk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3byfguliq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zxyudjve.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hweohywd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qmobiwns.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3wjasmdvk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qdctpgxq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxyuxqbk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3odqbjwdf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3iytwxoml.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3swmnrjml.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jvxcdwmk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zjjfevpy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ccppshhb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fdurawbj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3guwaykiv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bvhjzscf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gusgqysc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qnljwajf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3duqwtpzr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fstmsbwe.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3janmsrtt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3zqeeolpw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wgvmwsqh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rxyclbrm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jeqrlsuw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3djzrfxbu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3scaqfhrs.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lsskropt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fdovbwxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyluxesd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3lwfvdhsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcmjhylx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3qlentyil.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jcgquuso.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3spnoksxn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3gwqotjap.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ribktcha.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qqurzjqb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zbtheahv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmlsrgaa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bwoalfrh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qubgqfej.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ftyvbemv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nexywxpl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pkoepafk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qorpankz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uuqcswsl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3mfpyyqpz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3mlmbdmva.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3eztlucsl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3powkgtnk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3dhphzgow.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pshylzhs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ivwrbqoa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wsiuzkbd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zlziilbq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3mgjdmlki.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3iunxdtla.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jpxabgph.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3nqbfkqgj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tbdnehuj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zdhoewlq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ityoipgn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ueecyjfh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ospwojid.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3muzbxukk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gewtorgi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hetnwajo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3otfiwrya.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tboitthq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dtdqwumh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgliyqix.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bldanycx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ffeqxuxo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qvvemnws.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zkxoznui.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbdhmljd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cirxwxuu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivzkmcul.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xygsfsjz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xkusknpb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdcmuiaj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bwyfexhb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzunugla.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3texpdtxa.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yrdsunbm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ywxfuszx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bnpqmnpr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vulhiwue.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3payfscdl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ugigxwda.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qduughhg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lslrvjdg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3grvwmqhm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mmznjftx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3innpgnsi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vufdyzyr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hhqvfibd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3felfujhz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ovnmhvsp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dlqalzcg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3quarhzre.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mnqrjpdt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wrsldqph.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3logdpgqf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ppmwpgam.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wzjhlzwo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cqzoieec.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cobjkada.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wkkcyoti.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xmhdcasa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynvbftls.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ahiagpte.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3pbwdpvxd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xloczqgq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lqhsiwwh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mudnmlkh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3czkkfkyz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rtjwbeae.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fqcdlgnk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wckvucqg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zqcfgspr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3isxzsvnv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwzjyzik.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gbvcyquj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3egfsldes.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3akbgphyw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zvfsxfjh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ditxscmg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uuczvfuu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tcplytns.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fcebpukj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3slclflsg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wviuovxs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3oupemxqs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tagaqngq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bloqiyha.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3sochiuqp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mlmemiey.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3liyjgcgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdbiznsy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3bwcnchqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyxxaory.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3tfuwjode.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dkwztiom.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wylaummc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vnhdnppk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfeupsdb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3efwklspa.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3exqnifvn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3stzfdjqo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yvxsbxwy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gsoweogf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3csymkgxt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3auadjzkz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmztpovr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zhbewseh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3anxqcttb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jwfixeml.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ukzllrip.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ruzspvgr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3eahufxnk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ljzhtomk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xhvmdlya.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xvczzrmt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ntuobsci.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3oygligrj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fnfcnesj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3onbyarwp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zqredqof.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xodkytjd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xomektud.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bbnbqpgu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3akjbwvoc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zxvrcxfd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdkmwxgw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wtxmjjdt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oncxrtox.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ifobkyra.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xyoqfowf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fcejzaqh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qybqogqu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xfccszfy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zxylwukl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3texetrse.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mgmrqqmn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fvzjelna.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhjmktuf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mfebvvmk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zejkefhk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aszxxdbw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3feclvngl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gpyddzpl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cnugoqye.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3nnnwtcbx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nikulfre.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ehrkwyrt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3bpvfezbd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3inhjdkko.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3srxsalqd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gzzksnvt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bjrodpmn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mjnvfmit.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vropiijw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3qnecezad.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3reusrfhd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gsdsnfeh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3cwjhpkze.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxlotjjb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wlgucigt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cokspvku.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ljuupbiv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mckjppsn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3iupmvzsh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qmhepdvs.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zoxmyodo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gmdkeeqs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtwivapa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3uufsxmhu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zggutiqs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3sexlqket.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3txjmoejb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3bcrnpktw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xqwnkjup.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xqavrcyv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ywofnfoc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3suuiquaj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xsjdszsk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nojhndss.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ebldsfix.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rdqkbjhv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sqdsipam.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bewhdafl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mvlwmbqn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3kkjiqnol.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rwgovioe.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocroirpy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uejmllwe.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wqtrehsi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ctkxuwsu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ngmqmykq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ufuaqcgb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vpyobzzt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kytqxrin.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kjekylgp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jkyrrvps.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kljiohqx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbwqtfty.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wegsasuk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3piroagcj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3agaifmem.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gvvvnzst.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cengjymg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hclzhels.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tyojnvyp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pqukbhmh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vpxtnskn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3myxznhbi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cwxpazep.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ponvrqgc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nqdfmzqh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fbxsqdfd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3thlvynfo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ueftooiz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3fctslaqc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxphgwuj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qetucgci.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kysubjit.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vdefhiwx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nqotefwr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3gycpgzpm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufivfrla.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3jihoejlx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xjjvbcht.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3scmobvyw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ovwemenc.html


<!-- 参考信息 -->