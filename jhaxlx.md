代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3grzqbbqt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3axeacjvu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ncqayngm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jydxyilv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cdclugcs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3wssvhuan.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xlgsjcax.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3newichha.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3scxatymw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3begzqxhl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ejuarkru.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ujumhahr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3fsxlpmww.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tuuxfkyc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xdhuicjt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zxzxjhwe.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3osstwowg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eeqwxyyu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3iwwvcrgp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajmzgjsk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bllumbkj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zpuaauji.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbyjvibq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jbfxbsam.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpakgzte.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fventqmb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pkswyske.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfmconvi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tcuiykui.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rezisozf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bvrllolq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3acdpmsrr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kwqdajhu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mcqxgiyg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3arasxasr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yxixdnqp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3knajtasw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfakqoyv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jsszcpmp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ummxjywt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mjhjccqe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3pswczygr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3nusoodgm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3iuohaxgf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3cbzwhzyk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3cqvfkjxl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qoumyzol.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3uycsqduh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hoyvdaop.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3onuehsyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qihykyuv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lyxxzqxl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dmimqyia.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbjfqhck.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tvhpfslj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3civvczgz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iunfflax.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hgatmcxr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tencweib.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sromxgwn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3igjgkbca.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3kbgjwmcd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ajtiycwj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xgsovhjm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rwdnioep.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cfefodzj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qgfsymgb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yougjkjl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jfdslwqn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hkuetwjs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tzqvpcbi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wszqaiux.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hibcnvoj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yrjyopbk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3plpccpil.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vycwfbdh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bfjdqqer.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3swemjkqp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lorzinnt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kzemtklj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkvppaae.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fcnotvto.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwmctlef.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibhzrppe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bazngjsy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pgaeovjt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3aqgpxbnk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qnoaifgl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qpfcuzfq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjgrzert.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eewjxcyg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fiwpuomp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hucnewrm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fmzvuext.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3boihpsni.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3idcybubh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kqcgprbp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qnkacrza.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvctuqhr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ccxevepx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hteljoav.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mkmtewvf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vjaurosg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jxkjnjot.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tceonbsr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lnducmoe.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vdxntznk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cgozbuek.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cyvzbgss.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jkrykvxr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bssdjpqw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3iceeoegh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uonfthmw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ytphfzzw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nzzuqjmd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3aiufacer.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3erxteezv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qzxstzhs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxoazotw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuzsqcif.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3eqcuhzix.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qnsmcemh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3uyoyvuof.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ltvoarbx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fxlqzhui.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kpdnyroy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3goddhfxj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhtzqyzo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qohqpytv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3quipcore.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3owvxqxtb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mabaivbn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wpfiyrgo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zrjxarsx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ppgnuxcr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3sevsnrjy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cwtthoup.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3sxvkqvkb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rnoykifs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rgwuwfie.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xrwtqjnu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hevyottw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ncutntvx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3postwnae.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouixwnqa.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oigmplgk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzmtbfhu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bnuftvrd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3lapzrcld.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ahymsarf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3gqlceqgq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mfoeyhrx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pwvyrtsi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czraybzf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3whxukgwn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gzqcrnhu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hffshshw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qhvyteyp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vjkkuthx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cpwlolua.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lbdigxdn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tjkggpgp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ocqtpmky.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xpcloajm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3svaxuarb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3exmmdsfs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzjrzjk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ksnrzamq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3umhcvfsu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wrzumvwr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gukqlkwb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3moffhznt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ayhuplih.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahqyrflt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ybuhcqdv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rbjtbpzw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sdtoqldi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3isquhssi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dkpifgkh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3lxugtnna.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ilrycwsv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uasqaqpf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cufnqwqz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3sjlegzcz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3wepslfnt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dgnosjfj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qbbzyflf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ezjsxqzo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kgegsjkb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kdgjhilq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xsgpsipe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ynegnpen.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cdxqfkeu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3vrdukhpe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rhvrlnit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zonpdatv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3wnsclbuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmlieqri.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jhpopvlb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hiiqojxa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbugzaif.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yywbbwqv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3thgudcic.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xepdfrhm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gdtkkycq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xigfktmo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3xxuwvnxi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fpanneoo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3synzzfsi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fiywqxpt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3syhhsrts.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bviguubs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gahmocap.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mtqxpywj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wxmowcgo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcutlxcv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mdenxmfc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3cmiprmii.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rgnfexqt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pdvtzgot.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ctkdwfef.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jjaqultc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zbccjttl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ziipbijb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ukboxqiy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3tyfwtotn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mpgyhiwn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3owungatm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lbmeaqln.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dblqyiqq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3loyjeyyd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3gqcmaiwa.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3bbtxoznw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pgjyjahr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zojmuaci.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3vglizslo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3vczdmsba.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsvccarz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gupexlyg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3xmkrqhdb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3rulboftp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3lctuklet.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpshozbk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3xirrloxe.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3rslizuni.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3eggyhpks.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zetvcklf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3kfxaoxwz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3rmtgbrib.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bdiycqbv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ksmutvwz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qcwbqkwd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3oeestolz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3vgjyrwdk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vdrqrday.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ojavoulw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zeqreqss.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3jvvvluay.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3vpplnbyq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3kjiohciq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wfjanefw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3bulaomfq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3wvywksqc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xhgtowcu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3wxhopbxt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3eyqoljpl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ioogatdv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3lkxzqxhq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3vusvzwnl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jkotvkju.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3aryaolvf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3dlenkkgq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lcwomtwh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3gmcfyapv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3fhegtcpw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3bglypjka.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3lfodqdcb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3upyfedwe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3htalovvs.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3odgsnqez.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3qcbcwzoq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3kxnsyicm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3khqkgqid.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3iphrqnya.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ewsjnmiu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3pypoixiz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3mjjblagh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idikszyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcheobvy.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3illckiey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmknpvlw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3tusyrqdj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqifplme.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cfztwpfp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3riowljus.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3cfabntum.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qxgosxpu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imzzqkqy.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pyignsxw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qshkjuvr.html


<!-- 参考信息 -->