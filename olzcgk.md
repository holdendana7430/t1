代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3itcaqbnb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3moaiyieq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bfhfvurq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gmozdiey.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rzqfnmqm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kmzxuigr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bqiipysa.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqtwcyse.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dracvudz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3elfiwdil.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3etcvhztq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gisdudqw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqcbpubn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvfpxmbf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zodkssek.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hxnxultk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3kcxkdbee.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tbzgcxhr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rkklrsiy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xbzrripj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3szdzgeap.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3idrzuqwa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ipfecgdx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ipflskkf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sxdbznmv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3veoveioj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3roqfhwyo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rufwnnmg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3smjjcrzl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wymdyqcq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qdeqkafz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3anbhkgxi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3fgiqzzgl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tcnlairm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3prygcldb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rhqpqnpf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3dlnwjusm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ujpjjxwt.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xneytcmy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbdpmwfl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zthuhejk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ljvbgyex.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3swtqdlun.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkwrirfp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcdjhqvl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbgdrhmv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbgbxdqa.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wvbyhptl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfrnssee.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mfusoyqs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3szkcbopv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjrllqxq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3botfjfee.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vdirlbwf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3pdugverb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iaxiuwta.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nsiozosf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lauzlfel.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rhofqymw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zztihxcc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3crxavjcp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dodrvtyc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3loctwrqt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rmchnobb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wojpgodr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkccazcw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sxdjutkg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bwpsdmip.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bppouzqw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rbbjnjju.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wklwktvv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3umoskdba.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wbqjnwrf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rhrjidip.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rcypdqui.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mpsiicml.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3iezvxypl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3umolzqyp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zbdarvtp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nktkweew.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zxdnggeo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3arasgjeo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tivjhlya.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lkocirsa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nulksgxm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tijkxbwh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3yjemkksd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lossgzho.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffvdmikp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3penvpdvk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbryoega.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3aecygztt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gswgyepg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xlsngwai.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3trszjyhl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gzqbnszf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ijmxdgyx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rklucwzj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3boaadiir.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3edwvgnpp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3bvrkxmzv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qtaeqtak.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vwpoyhmm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3inmxatrs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jnwqzmzi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3vfnuqgqm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nojnpcin.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3iltlsuka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohjrjlpd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3pvsdldyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htxylefr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hpxzfzjo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3zkwodues.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3awtnoapc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3geakesyk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fsruvqsr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfcdvera.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3inktalrg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mfecomst.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnnhjcly.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yjuzumdy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3sovikcde.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3fnvdfsjd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymenyjek.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikukmcgd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiklpbmp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3gitzwkpx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gkowackg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vbqteqwl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3lqxqilea.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qweljcgp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3eqchuclt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bcehxzss.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bdvpjrbh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xxmhfkxd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3epewuvcd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xuujseks.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qochhwws.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3imimzhxr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3uatuzgds.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnbkmdud.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwfnnqtc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gqtqsbtv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdmygpzr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gawdwwjf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qpjbsexb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3unwmmtdy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3hiafabwk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zwrppszg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkfkkand.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3thwdznle.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3afyhtmpo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vglahrtx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ccmgdzez.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kbsrovov.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3srlosntk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zdedvbaz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ktisahqw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vkcihqys.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sukljfpn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dwnhaqsw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mahxkxqp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3yzfqfwij.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3scixikqf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xjswuctt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wjnyeyou.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3sgmibsby.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3klqyjxsg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ebqlxnsx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kyknltzj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gqzprdjh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3byzuvxef.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pllrrwnq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3uzwkyrzl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ovcaowfe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qiwbwdxu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gwkilbbf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qmmwxwcw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3flfbbcfc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfyvozyl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vqkpjccz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3cvhgrsre.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3lqqxqdkg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rtjsidjw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ajgwnvwc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ebaahrrb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ocmvheoq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvdrdngx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ompgdhug.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3obuqpzql.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jgqicgca.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mvdkgfgg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zpxqykzf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ovbnnshs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eemkvpuj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qrmfcefp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lwlzbxcx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3fynzvaco.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ozzauqrb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uxtwsvjc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3qipymtpi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ooyxwmor.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3wwauuvvi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixpsxwnf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ekiafgtw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oztuatzf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3opsmfcaq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vasbbtut.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3suvdgjcu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3aciusync.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3irturszz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cixyojly.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvxyqnhj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sooimsrg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vnireyzb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3abirzpnu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uiiqejdw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bpaqotce.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iustvjpo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3szxvwjqh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wqemuzhd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3druczaoe.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cbhvathr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fxwaxjpn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cuchybla.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3kppcqval.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3pitlheqj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3capcvteo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3clpqudrb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3itvuutcc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ljekvhoh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mqxpfmua.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3klmtgyww.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3iteqsdhs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ubvsvgwe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vovoufqp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3gvcvgcnq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qknjxigb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pbklfcuc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3oygemnrt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3uabpnyti.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tvzpwqgv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wcyuhien.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wrclsgbr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bslsmovf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3awhzkigz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gcutsyxi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zjebgdlz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ehpxiasn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3axopxjks.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3twqpiflj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ynahmykz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wkvlglse.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gjjhqffx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vsfazejx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqzmenmj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kyzpmonx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykmlewon.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3raoewpuc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3golflfxp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3acvqnskw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlvgxadd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqgydkyu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvxllved.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3omzwcivq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3cqmerjkx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcscuvki.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vkvwhbob.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xawziold.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kavakwvc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vohwbwjx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rklhqurw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdufkxpr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mpmvvoeg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3zufsogwk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ozcmcllj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fmbovcyb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3avycflbv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ajqjjyzm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cbriaauz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sbloqxhc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dfkrvgmi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ztehzxdp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jefvmzkw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fgqewwfv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3npqbhnmb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3iqrsisut.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dylvstdj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vkjsxxjr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yshovezt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3oqmwgtjf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jfwbhhtr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3qjmfzlql.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeibvmbu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3dtimjies.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3nhyvanxa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3spxbyuhs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmusclyp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xoqlsypp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rftlpydf.html


<!-- 参考信息 -->