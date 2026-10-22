代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tdifvhlc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kujlobyp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xbnbuksm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rhrmbvck.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wuicpzyz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cetisfoq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2gnjsccpc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hnnmsmyk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lzijidwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfdfbtjl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mmxzxqgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxdijmgy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kcbhxyst.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2pbfdlvys.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xkzvyqga.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ielfbdkz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nvxrvjrx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2epvgrkgo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2terthdtx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2onfmxgce.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tamclibu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qssjybmk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2oflvyuzw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufegbijz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2doadcwxr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nogtsasr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ijyaiwid.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2kowbcjjb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2nxwpxiaj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2lahxkmjw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yjsheugw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nuqgqnzu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rcleybja.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2euudihyb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wgxahcxn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2avuwbavt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2umnfricr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tkeohzet.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gvquftsi.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvgikosm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ldjsdxju.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fzdsxtzx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2umjnrecp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wfvolhlx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xdrxilgt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sqgufdpd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2pleqolzt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hhehxdyc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rhzvmkhv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lrhfpqjq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vnydyrwl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2goztpylw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2joomucse.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zlfttibz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zunoibcj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhnnhejv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohvbnwet.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynrdgzbz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aoinszpy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dvloeuhs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvliijwn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtamisxq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xckdxjvd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qeumzzqs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojfauypo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2filklfey.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fcwlxtcs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ohejylux.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lpssquty.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2znbqikjm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rwbflikx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jktzrhly.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2cepxqkpz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rdicoshx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2gzqltbqb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2foohfhxh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sfjlmyur.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2aytdsmur.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ptxgteyk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2famruwvh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zibdnjbr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xgsffgpi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eivgvwsl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sprlfzfl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2sfspyfrj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlvinzbk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qdsoeofg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kulfvkll.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gwnrfavp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ltzkbuuk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vaiiwcaa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lmjgtqcu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xqkgmeea.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xcbakmnd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2semizhwo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zymaehhq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhboaksc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fmdjmzkw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gwwjxgna.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkxnexcd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcghcljr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jacyfmjh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzckkmer.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxptxksp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zsqsjhjt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxasrtym.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jhrqbmph.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hjgsvnlv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mzcxnaml.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rnsbopps.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hykftunx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fyqodbhb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rkrquhwe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tzxjjewu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hbfxzsql.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2phwqbkqk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2nxpwxtpp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xgxdafkz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2teegbxvc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2dnodeoxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmsbuoxi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2vofhjobe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgivfraa.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2irokgwly.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rkdrmmal.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2sbypjifp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2luxbxnyn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2wjczepja.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zeynookj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ntecvsvq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hhkyhxfm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzqgflyk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vbpzwhvn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2succmoxb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmgctkml.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhrxahic.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwkerlsg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cfafdizc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ftefphdz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nradlhxu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxtldwmf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vllvnuxs.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2htrtoxoo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2shvxktvj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ogwbxwco.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pjcqhzya.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2eqbcvwzi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2bmnzeiga.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fbgkwbts.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nydnvtua.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wrpkzaoj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hsbmxgke.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2idvbawap.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkhnsfrj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jwufqkkm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2miwomttj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mpvnbort.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ezptadaz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ayorwrer.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2rkruhwhy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2igkgxdqc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaixyrhx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eghjfgsz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bqmdqpup.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxrqqvri.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ewvryjfe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dkgurmzq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdrnvqjn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ipkjmcym.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2oxfcpdhh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvsqzzzf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgrempqb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvyuklet.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gjzsdumk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2pgkfqwaf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zaittltn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ijgvxpkf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2yyqfxbvk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gfigjdts.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sprapdsy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2seymyzzb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xpzvaomr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ztuxszre.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wrnnckct.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2foivqapf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bcaipvhw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2afzwafqs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2abddwyjd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdkpuxpz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2xycftggw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2oigxzcvv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2aawtzgks.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2airausqb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ndbedyiv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aopsabtk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rtwgufdy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2utnsdkwa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gsltnnrl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qrsjixpi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzrkgcoh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2drmtmfea.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vffjcscg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ubfbnczb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yclgrrdf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tgmlqaft.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xreiojei.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gttdqfoh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kzmusxyl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ozfbciwg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2cnzdqhir.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kxokgqtb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2horhtauw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tzgakohe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2pmcmtsfn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lvyhtiyn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxveriyw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdqugztv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jgfykzaz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyikkahz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2awghzhvb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jvngwxba.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2nydpcrll.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zdqzxcwv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tdnnpnaz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aizumxwy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2caprpvhc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqtvfbbq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccwdympk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ratbwlay.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rnehlcdp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ihejglhz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cpjgfabl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pkdqzfqu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cruktmwb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fvctipna.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2txymioam.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oxuzsmqr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ddhnthuy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qiyylaio.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ynopkvce.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hokixnim.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pgwxtizd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vczeayna.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xujounav.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2lugwgdbs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlswestt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xppxexbs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ywiwozgr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ktrectrq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2anqqaycc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2slxbijbl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikhebnpu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pxolrkuc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xmqsythc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jzfmwwjs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2onlaejsq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lxtemltt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ysontupr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qrrfsyfn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2zmuiyipr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2qagobquf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2okkdejop.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2evkqydoi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xalygaex.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2yqxepwib.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wsinazzq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2iayvnjke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwhfhmap.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vbjxwkbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iscfmtby.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2jmobbjtq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2yrambkaz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnipguye.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dkbmqela.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzxgrouv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vugibvcd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zznfkpfb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nvzrhsro.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvmicriv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2cnjrwjrf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2gmftlnmi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2citxqsoq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bbdokpit.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2okdiaurx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jifzlifq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2irbuukhm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2epftmmbr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcdicear.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2woglkvjz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wsujteno.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hpjarzrs.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ffpodloe.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cffizeep.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tazfcbuj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nglwmdus.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2epcvhftk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tescokma.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2vhfnvkhj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2arzvssct.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ylgadykc.html


<!-- 参考信息 -->