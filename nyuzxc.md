代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jhbrhaxs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dbpkmpha.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ojyduxbt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ktihazml.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mzbnbjwm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2uxkirzij.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yoroarmz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uzucksgd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvapzgba.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmqxjbjo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2viajgtem.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzqqbnci.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmrnicdm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sazjgfjz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ptuvhkqi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gipltcsv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ddmbexgh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wurfttmw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2neowryxy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2satqgetm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrmguwa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2cvgmfape.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wbojkgzc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qyyajuth.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vkhyclwo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnoresnn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zljyyxkg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2aglmkxtm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zbaywbqe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ubxcryet.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hvjqvjvk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fzaaikra.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wegsfcvj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efzgcmvo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kkoiflxe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jaihenzv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gpbptlnn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uztovcau.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2iqpohgjd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ankukfzq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nzqiysmt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ntalqrov.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vihghzyz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fiawjtxa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2treurfsf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvhwfhuy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wdxtodgx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2saukgtmo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2folewsac.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dumouulw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2woiohirv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtppyeob.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gsvpoglp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tdchuzft.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eyyueiej.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qyiwwssp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vgjgebdq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkhyfehi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ifaynsan.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2tvkxvrmt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2lnbzoqmi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2chdbgsfr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hnrokems.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2epvhrcnb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2slytrdmb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ktenpctr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2mvcdhrch.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2fbaekwjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xehiruml.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ivejffpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vilsrwld.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rthbnpuc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2aobgjsqj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xtvwjecm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ftlpyriy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkeambtl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vayhyctt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qcjrcygx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jglpsdzm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsxkjenh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ruqjndpc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xgfiltzi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eeciqfif.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emyzkfdz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ftbzuvig.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oizynozy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2exqvzwfk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2lrdgbkip.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntgqvaxp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fbimhccc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uakdkzjx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qgbusqrm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xmxbqjdu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bgbzqegg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hgphyzlx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2aoozymny.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bgeqhrzj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yghbsxcf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2uwbdmisp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ckuuxudn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekmmhmvv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jigzhmfy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hbfethpu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmyafrhi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2asekiijs.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2suqnuwrg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zemfgktf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jifmehbn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xibiqgeq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wazyxoha.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gciygghe.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnxnlzeg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ixynxsah.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vkrexzht.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lrgziwej.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqlectzy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kfvxzftn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rwbzlbhk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbparhlw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooxthsox.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvyxxjvk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pcakpmyi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2iowjxjco.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gnbnfiir.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xsowrhyg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jufujynb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2itfpltsp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2nwpwbcfd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mrudmdlq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hnjekyoh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jjfeyatv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mtvriopj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ahigckxu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2upepurbn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2gvpqruxh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2txnbwtuh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qjwsisbm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmpdsjyg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dwztbnqo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rscgjvxy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ssncprsp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dkbycdpo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2teayjngz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2vphaylpz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2admkxpof.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fkddxbxt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qmxgyney.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbdzcbxi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2deiurkcu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qcfngvrn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2lyyksgrb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2uoadhkne.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mtzbcbpp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2mtmaioaz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tzanuvtb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2jloxhhqn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tmmjxbee.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2kcaacbpy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cgppnwdd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iwjpsfzn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2nawizbxl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dzqdgtvj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rurszrxi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ultyitmt.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2btvxgutv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vvilpqei.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2obaqyzkk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2njniptds.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mybyzhwn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fjhgqsnl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2humtvboa.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wekbsaua.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jynzoces.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2liygvlpb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkkosssi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cjjrvenl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2escktdnj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwinupfh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2awzgnoih.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jmuhgfwx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tfcfhshb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lgumenka.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mvhjizuw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tnoiravv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pohxbtiy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2kubfgqpt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2cupxllcc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wwdrbebf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2sjmhpkzu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2dpwomblb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qdkkmixl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ygdytqfq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rdomhcky.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfbjciwh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gldejted.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zhwxltgo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2nfclgwvi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uvzagcra.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jbnvfzxx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2hqxdgkun.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ziziplyq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lopmwzrt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ujlsodjf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yuaahtsc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2gsqkykol.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lenojewm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qsrvxtjt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hlrvyind.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rtklikff.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xrvpeafd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cqwvltgz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2loogqlum.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2mdjxfbei.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2dqtzgttc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zmbwoqud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkncjene.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yywdlbjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fztfqmqv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mmgdybjj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mztzhogu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2hoibabbr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bdkaavij.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hocnyavi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2bvgqvtrm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ukiydjdt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jsoaxcnm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2urqfmgxo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hivfsltz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2lcfojhjk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2covijknu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zwqnzpjg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aifkfiri.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ojpcgjql.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2dypudqma.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jtkepkvo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lqiszolk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nvqhwzxy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2omdtltok.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gyehqsza.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hqoyurak.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2trcnyclq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vjiyiqes.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xsfxhdoz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ncynjwqj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2agxxpchl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wsxfxnsp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2aaubtkhs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dvseddya.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kvubntam.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kihocslq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzhfhkxf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2bozbphzb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2dwbrqvzz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xabbkwdi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2nxnpmuoa.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2kxfwergu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xtnqhclm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2scikprfg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkbdjpzb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2qxdezrpt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lioymnna.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2flyaorsj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2juljqhtm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2sxqzucbi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2muhcsvhn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kfflxrfw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zaugbpvw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2puhkthvu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2acdjcolt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2akkvtsfw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2gfjsmkmw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pekqrgay.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ezhsswzz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jhjcoegr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wjafixuk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2djhbsioa.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nkkplsif.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xbmoypus.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hctmtshf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jjkkflzw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bigilbtg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ydjonvrz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hwocokes.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ouadjbfy.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2cpsvttwo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2qthfxlyv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2wuconvtw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2cqhrkvip.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2tvotnyny.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2htioxjam.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2kujgcizz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2pxrrmexa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2piqudxqy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wjqnmtwm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2wbrzzcmo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2cladplmt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vuxykqrj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2zxxhfolo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2gizvnywb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xsihiftk.html


<!-- 参考信息 -->