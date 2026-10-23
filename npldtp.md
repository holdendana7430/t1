代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rlstgybf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uplxmbpd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3modzewed.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vswdzpkj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tewynvua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugdmcxbj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qltuggoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llhvbwnf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wojcabkj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3mjlegiyj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3owfixyzs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dfvmedqd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kmktdelv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tgvkjjrq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tzmurclt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kwexjjrc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nkrwuebe.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nuvcjbvy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ktwogsye.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rfcxqjoe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3orkftkfv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqgfnzxp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kqotidby.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mkgiphvn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ifvpzibt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ptxfvlyi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3baqlyqsv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3whvbcjfy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gosdxxtc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lltpgmwb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sbozdqgp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3yoacejgj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3btugsuvw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uputdspj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hruylwyk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gqostrcc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3whgtnxbl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qoopspce.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3orazzfkp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wwalcknb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3olfrilaz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dxahohil.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3baamskzx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qtqgympf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vybfptcz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xbkzqvnr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mqryvayi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqqdfwol.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzuadzyr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hmjgtuwl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3dhnzjxtr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugopycas.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pytmdzaw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cihakowc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egzrgymh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jgtzvfoq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nywittbb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wdtkmtan.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nfijkavo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjspxzxn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbfxuupe.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dfybsclp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qaymufsi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hvcusywv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gdhjsghn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dzwlrrtq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jwvcfguq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vogwwopu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3psgxgvco.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3llgytqvb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3alowcngt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3iwfqxogh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3tygcfdyy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3oljsnhom.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zthwrvne.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yoprsyao.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yeypdyef.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3axutqxpe.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vyaxkays.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qkcikzzd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fydrddxq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dekklsda.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uicsslbp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zgioaucd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zrlinvvf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ektvxzco.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3hxefimdq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jovlttbc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wlhqrgbo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ambkmrpp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qebibohb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bbpwymth.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfvarfhf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzdnjpqw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3lhmepdfp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3medgfwop.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awlxvxug.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itfdxozy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3salhlzob.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3igcetinh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gcqwnjtq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jenearpo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lvwkoauo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tcttjysf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rfvucuck.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxbyplyy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3npgiarrl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wmhgtdsz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xiokwpth.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sjqbqgmb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3djymsrai.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hyqblmrz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3fyhiqufj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3btyflptw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3doutxouk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3yzlqbugt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdpbdbxf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rafqzhcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqyublvu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hrydkcwe.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rgskafuj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3dvcoizxf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fwwiqfoz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhgjthmq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3leaualen.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zlzszjzl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ohopanao.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uykrwtie.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3svrxjkph.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3vfzbodid.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3degwpxxh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3alyflnoe.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vacbhsde.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3outvqzai.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qaulirpt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lnjikgpx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mawnbqhg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jbbwqhtl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gpxlvwfs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dmlelbtf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ghejqphv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3efyeuvgn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dwnyzwpw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3onzeyitu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cpvvhrmp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ktttywmj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ztrvdxvr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3efpzclgm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjgrqeio.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iopvjedn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqalsvbz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hwgnmspt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iknyzvbj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ukjsbyvu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3paxmeplb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3cctycivz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mpxyojqs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkbsoogm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3awsmhkwh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3amymjwrm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nztapkfx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3dpdblyem.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ophskslj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3fxqgnoqh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gyfzuggm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kdzyxjgx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxgzakcl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igxtrzqw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktrgjazw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uvnqwxec.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3btcgzokf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3thkkdtes.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3lrtcxzjm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3klxdtdui.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bqmltods.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mcaqixnv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ctdhqnbi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vlaatkxg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tsrppewm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3svvzqfam.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ksunurzj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3icwqljqk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mhtkdhkz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ityaigtz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tkqpqtga.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ciqcqrct.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjmkoriq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hqakrxzk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ublypdlk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3uwrkzony.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqssezdr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3lakqmkmc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gblajlvs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dmpdszrl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mhukjkqj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyruaueb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rafwngtx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3corqyaiy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3lurgixml.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzllbkvp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3occekcxq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hgyfozau.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nxbltlas.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zbvintjl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cxqtlfcl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ubhhnzty.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ouvuslce.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3etrczdxo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3swrieodc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3iidkqkzb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3eugrdhes.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3faxmarde.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3oouwrehd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gnzujceq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uepekvws.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cuseywbt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wlggjvwj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hacktbzc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3laetljbk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gifpibea.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozhlhsfu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fngsbppo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyhhsehq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ymsjzpsj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tjkqxrrb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3euqlzdac.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mocknbui.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3udkhuslb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fielkaay.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vwzgnclf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3exmkinwd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qqogpafk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wddxszru.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jnhotxos.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3rxfmttvu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xklhqmde.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jywfwekq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ybxnnwkk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mszaprwv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fvgxxnya.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kokysoia.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cidxvzmw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3rubwgbbo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ooxevmve.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ymnrgvjq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dsgqetbl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xrfrfvls.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfsmmnoq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3anfduwps.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nvafaqbu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3klwncvco.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mgszpetr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3fblirwka.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sjaaivgw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qjbsomwl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3elzwmibo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vfnbmhhh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3othwhqnn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uxnfquzg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3bzchvwpa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3sezrnrft.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3pukbdioe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qeutyflh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3toriskph.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ueflpmsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfprnhwz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pubkbaxk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wfdseyjr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3szbaipow.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdauevmj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ympeegxv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qctpaojy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jpizdcpy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jbkflres.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ugxyoiqm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tmakkfmz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3emibihur.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nvfakhcl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbbwccuy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3znmorabr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aghucghc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zaxwgdll.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3yvxnujrd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dnyqzfcx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cfxkfbxx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3obfusmbg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dyfxfxjk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3evuufogn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wmrbezbf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ggfbemxc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3szpnduja.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3uhrycbll.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hualsbow.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3yvamclnk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ujlpmjyy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kanhiutq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pftyhnpc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3botxfxar.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3loltgdto.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mcexfpmw.html


<!-- 参考信息 -->