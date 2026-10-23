代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jrormgzr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ttdeoybc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3knglxbpe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sknqakzj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3atspibla.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3cczaefhq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3javesxcm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwzjkluo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmovibjn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xsmdpkue.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3cielsufn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgvmxshe.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iiyokuly.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zmeamtnm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wunvhiaz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bqvgdzch.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ismlftuo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvkcvnvn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fbmrvvyz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wwsxkade.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qalokigu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zopdqsrr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dnabvwae.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ovurramv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zwygjmpe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3sjhtdmnw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3orbhvvor.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3npfkexnc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3egpaisrw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3uvbwthoz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3muunsyhd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3waxgavud.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rzewcthl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3strvfitw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3luysphve.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sygvezaf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qrjzkofl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mtivxxad.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rtleufqt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jekjlcvb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zofhwqtq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkwibzhb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qkezbvxl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kjyduznx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fjlzpsmj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dvytiiau.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qycbdpax.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbrknvkp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wyvqnqpq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rzipqsfu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3akgbmcel.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xywwdiuj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xalqjwjp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsfsnven.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kfwwtzzw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frfhknty.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdvwchly.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxczegkt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tkbbojrh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqwagtos.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jhflxygm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqhsmvcz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbjbftxv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3irkkolyq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bopughta.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ulvquaxj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3fzjxtviu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3buujyvqm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3sigaizma.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3leihvrec.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ryfidadi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mgsopqvo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ogsdrmmz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hvssxhod.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wcntybko.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3pdtyugms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btmrlwfa.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3eoyeuqal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqxsirmm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cbzdasrd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3nnpcwoge.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhihpqkh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lmmehnau.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3znhrwifi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvcvugba.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xbmdngsy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3meslswsw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcgjsmce.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ixzcyxsx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3owzrwgko.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlqoeibk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yitrghwo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jhspppmy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmnvsawv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ddpnvhif.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ianrljdr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3eyfsoamy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zdxipblv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nomhfanv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jbrqckpj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xkkxjggq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3snhepxnc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3htepojvm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xvehwgiq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cguyckib.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xocaimqf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kjzunrjz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jiphcqwx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fyksqbhn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3amuoqlhf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3adlvvtte.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlxybujt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3osmzrsrh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3inhxdbwz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sdtrhehc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jmzexeog.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3gywvhxar.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hijyvkbr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bpfpslsb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxhicmoy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljfpqdgz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uvqfouhz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cerxlkth.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvmwceww.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hdfvljsx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bnyaglua.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krtzlero.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dxgtcmlx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rkbvkgsz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3esqqgwpq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3iqhscgjg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3cladaphf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3evddmkyq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dbfthdyj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tiwpbrik.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3blmyqtwm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ocpfrlao.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uqoaveoj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3faibwcwa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3heasvskf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fgnhbwgi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3omvsercs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3tgmroiij.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hiptggic.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxldjdcw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwamzpae.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3biiwyzpz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3oljgaljh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hwazsbgv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hqrcqjta.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvsnwcpc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jttzftoj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3dndjbysn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfybvvcm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wbxzxsyh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnlazhgx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3crwhimmj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nrxzpghh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ybwxpanp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mturznzn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3frzyeebx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fhksjlhc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fwxsrjqq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ueagdfpm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fppduzxn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3enwarkle.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jbyapddu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3slxjgxda.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3whvoqdfm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jvnpjqgk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xkgkjckf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mggrchyl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ichdapmt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwremlby.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3awqjspil.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kbbwpolm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mvjtjysv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3humedmct.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oleyawgq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nzyjguau.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ktpkflyy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mlxcylbu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkaguxsx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzxxcptq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ydpesbws.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fgrxlfeq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ongdcigy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3smekvmaf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ludaefwe.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jxiqbjxi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nhspgjru.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fdcsufmx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cmxcjwbe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vapqdpyz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3obrlyhwe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3errdfdwq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3snwclxfo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ddghytig.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fgtvlxge.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hcpsyjjc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qhbxoahx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3uvvtwzxa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bwkeklwo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3fgimlnkw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qnirltzi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nzsfgcfe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uglukhmd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jsyyxuqk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nhhqkicc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rjmdmnny.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qjwjuupl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3gpynsccl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3rwfhhxzp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3odopfdry.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3sjyaohed.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jiipptzu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ivaamzww.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ibcpylyu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tysaezqt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nilmjkls.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3unlttgwq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3sfwlfyek.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kisnaezm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykcmsrjo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jfmzglfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3faopkkoe.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mwprchan.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3govtyrzp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3asvajmkl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3daaaqhbo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bztxpcal.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qvjeauxz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tuwylsft.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3rnsmfuaw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3buwngggb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3fnvvrmde.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ttmeqlnm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xhscdzzv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3phnmlaju.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3trbkxogr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wtoiqsit.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3pwisjgdh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3pburkkam.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bmrjmoyt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3sksejooc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3dbciedql.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3njqkksbh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lpqruleq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fyloxkrp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dunuikvl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jbpzfakm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3dpqxdtxg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hzvypnfd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gdixnnnq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tcxxsccb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hoxltjap.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3soxaknye.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3prrtljht.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhumnrgo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3tlezjrul.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3asmyfxwn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3zaocoaxr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3cdixaofs.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rrqhabbq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3snerejue.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aoagzgga.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mruhiqoq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3xruwsjjc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zobphgew.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3syfconad.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkcsbmot.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lypbmnrg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3njsdvrgf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cgavhbhs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3isrsmfkl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cekmgehn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3zrbprxbn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3swfkowkc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ruxedjnj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kvtpblqu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ozvmejnf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qauyycyh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ncnxahvv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nmtjurzp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yknlprit.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3dhbnjatu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3supsiboy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3dmbnuctk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ypbabpsi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3yslgnpzy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kwhohivk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3qkarlamk.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3omyfghba.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bcplmjgl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dgsazzvb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3nzjozebm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3cbsqvjkn.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3igksmfex.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3zdqjuwrl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vwmofqqb.html


<!-- 参考信息 -->