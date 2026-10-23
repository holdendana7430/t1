代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zqcjjasz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzogavbt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ochvdrzf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vwkguucz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ezspvohm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmfjukln.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3nixsourv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kjqessks.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qposxoiq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oicxorlt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pfttdeup.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bvtywioh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3erbzdzws.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hkbzzyxe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qrmrrezf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hkmjagnw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uoqyrppb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3mpjxirjb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xqbbqszg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hqlmpave.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zluhkocm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kknmuchi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kytmsmar.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3urxyjjpi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iruhhtvt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zgbnoaxv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cgiazntw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubhlopeq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgvdlkec.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qzyxgkiu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ybzcioyv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fofzhfup.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xujfekjd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3tbzhxiur.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qejblerl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3khnpkkmt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rhcgzqnn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjjsheor.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3umbxprzh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfdwgdqd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjlvnxyd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3raaewanr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3uelenmss.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xmprxxow.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3zcwtzfmt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lyifflsy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cfnmbpbf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ugddpqtl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gclwrspl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3eetsqzmu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gomkoxxz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lyejnqrc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lcizcmoe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnxespcv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ngekconl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cwjljtou.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hbcsceda.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ekkoilbf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xxgdykjm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xskirlpr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3alpjnolq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohxoivuf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bxlqmont.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ollsrdqf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3biamkujs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xcdbuehq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3irhndcxj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3etxwhnmu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3akqpofah.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3uxfbsfnn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gpwffqmt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eoiagbis.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndubzrpn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3chotkrvm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3knhskxue.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlidmjve.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhmckyvw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3shlmcuvw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tvbxftgo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxbvsxfl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3glzczxwz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hpjqyegt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfrwkrzz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mfzwuqtf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lqtnyxof.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkoshxfk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3eagouaft.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rxobeiil.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3giiqvzsh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3lddczkqg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3tszurvkw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jmgmykvp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3thnoixuq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ozfkuudh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hepvxcus.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ixtfgnvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yiefskrx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qnldgxyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aedkfzxc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3khcsibgy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hjweifvw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxdixhxb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3eidgrmmb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rilqzitc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhzffpdi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zsotxxsw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3eggrwsfe.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrrsrvgg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fpgydfxx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3gjqqiidx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbeeivzk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thknfcqt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3cwcmayjh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zaapghzn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3idkevmwp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3mdwamkwz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gawdalll.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3uguiguyc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hvpdocfg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cehvpgma.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ipvbgrvb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ouytmoip.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xyznksya.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3knzbumjk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sjwurdhi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3sxiydbvz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ittshlgh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kgpxdtxz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvoaxyvv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bkhdkkvg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijyrvbuq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdnfzmvg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uknkvtml.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rnlazzfz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sszcsrob.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dibjcdqo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3bhsiwpxg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sgsbqpex.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsxsmjve.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnnsxalr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fabhcjqu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vhhyzpdu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3smisfvfl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jqsfjxpt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3uluuvgrl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3viqdvdqa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gvaaylnq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcwkbzxv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xjtlzsyr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiaivtmk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rzsjzxfm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zxailszr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xrmsyuqw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hambqstm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3aanzxpvu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kcbnkzqg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3upvdeobv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pgnrfxci.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rvsjtgyo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3masxyyma.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nkiqyzez.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fnobkisk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ckcpvchm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3skhgkobe.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrygtynl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsojmwmc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3nscnpnen.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3htzdhzxe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3nivwlriq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zhsemfds.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzlijrqe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3dbzbpxrj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xnedxxxe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlcmttaa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3anqdxjga.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qexicqyx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xuifjyvg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ymlommfy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gtxtlaxq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3rwljtnow.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zfonzehe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hemvdyqj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3syqzqirj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3psxsvxpj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wkrsqtuy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3dlrqlxpv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3pkumlmys.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kyegbkyf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ymkfmnry.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3dzfloxzy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tnfjkmrd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvpocmla.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3itqtryek.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crtbekgh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfamaifg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cbhjuuzr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qswdkbzi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ozzbyagb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bjywlkcg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3htiqhtxa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfaaqrfm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtbmejrf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iozbxcsa.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wlbnvlvu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ltqvqyly.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3seasyjeq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3thcmelix.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3dktwtufh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3khtgnoxi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ddmyquug.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xjkccfzg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xvqzzopc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uhmdzjzn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3iwivwlcl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3agfbvmam.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vrimdjit.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3tqmkvgni.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jbbechcq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ublnnzht.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3cuyrgrxd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3agwatoet.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdgfmovd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3rophuvwh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3tkwqrfoh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zvghxdkl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yyeywwwq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3djeizkdr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qylulfes.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qeawgkmp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lhokycdu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3haooffkk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3aaovsvhl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3hifhiupc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eoelnyub.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gurozqld.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3nqbojsvz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3xdpyxilm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fxowpkfp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3twxwuvhg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3yhablgtb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3dvlxjlua.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ydyhnspb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yufdnedp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtcoyedy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3flbolxtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chclsref.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3otzmckgl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3buexvgca.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpxvnfru.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjxpxsng.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bgwbepbq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3juptnnqv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rnczgezh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3xhtrocen.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3puwlvpur.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kbnktggv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3lzexdqrx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rexyshll.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjyptevc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3awnuhiue.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjsjdrzt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3uhdbcgtj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3cymyjmsp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3giveojwc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wtajzvfh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3hmyphafn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xjlsgbzr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ckgsrzed.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kapvcufm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bpoguhjx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vhtqknes.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3thmpfgnr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mtpqwdjt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfmfgvwc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3nhgyltim.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3opdqclcq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ilrofilg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3isxmatpy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwnmztxq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ahromuuy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mizwsgfq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyvpgkrv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3zzhileuq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3iuvyxocm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3gigzxguk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkawxvng.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsiugwey.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ritlfhui.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dubqbwak.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mfbixeze.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hycyppxf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3duoncgxu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3scpriwur.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3syvmmleu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xwmoodkq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mgnsmzpb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3cpykitjb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3oxjohqil.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3mznvtvey.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3remzkpjs.html


<!-- 参考信息 -->