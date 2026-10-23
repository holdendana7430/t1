代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3quamdyde.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3skoonvtd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3biydnawz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ntqhrejn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lpxkxalw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3iavodaqr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3obkqlzrt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rsuygobo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xujkzvsb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ozwgeqaj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3lenbaquw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3myxqgknl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3nttywijg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3witjgkzl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3czvebnuv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hddyozqr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kgfdyyyn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3thkkhxcf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3yxqsueab.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aareuxbw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3pngwopwe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nhvsijlz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbslpbgd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ursuqagk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ttjgnlmk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ufaiaien.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xlbwhvmc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kngsehtl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trttbfii.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhlauzdo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyuqbpho.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xdjcnmnp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3yfjacgpd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytelvpji.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eglozrnb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wkecxwie.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vpnnqltt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3afpdennu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gavpqhrx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3eedptpdj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3pshjvxih.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zerywyfx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vsrspgcj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yhnjqzrb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rcrvksiw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wtpbobny.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3modbfnyl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rkghsluf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvrbzzla.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hjamrbqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngfhvfst.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ravuydxm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3aymaynue.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmurrnvm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3addsftfe.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxtdcibv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkfmpouj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gleedvpl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ubxasnlf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zuflzoux.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ikcmzdmw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3drkxsvil.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3aucvnlsa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3doosyeso.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmwcuazw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3biovceou.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vkootjwu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vcmfryja.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjpxaxbk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qcvoowwu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wrcmfvix.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iiqnutke.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3anxhgvnn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3sdbskzkf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3btdsampj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bvqnhpah.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fxzcvhmd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nxrjjmyr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lwwytwhp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cyjfxesv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gvxacwff.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwkpwwrf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3szezywow.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wedvdqrx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ugmeygie.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rftumeja.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lyhovsqa.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qvxcqdgx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3nkqbclty.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qxqxltsb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjktncxf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3toolxitk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3krxbjdwq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3zkdwhpzk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mamedcsa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3yyirzfqh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rdijielk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3krxbqaxm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sztvoqlx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljdtwrki.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kaikagtx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wowcncfe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ovdwcjpz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3pioiuejz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wlnehxvu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ohnphbdo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3byqytagw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nxmdbjez.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ryvivkxj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wlhiluut.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tuiwvszc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vjpixmms.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ftgdbkth.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ysgnyflt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bppdbxvo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jzkfkqtr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3kkfvdemz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdowydhm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibwqjyim.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qatkkwcm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3umnacjjo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3rlyesigv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3nrjtoodu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qskghhom.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vaczzchu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmrzjrrx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jpmhloej.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xlmhioqj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3coskysav.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fcdqdkua.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3csrgprij.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcvsxiga.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yydfxkez.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3dsrtxwgo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xgaetbpt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3pquckuvg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ksobhtas.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tcbuefrp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3savlwqgr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dvziobbo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ijwpnycy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ljwsscdn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nwqpmtgj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3barulnjt.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dtbfomcn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xcvylpst.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpkqwkxv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oezonkoq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3exwnwdqg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zdkofbsf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fnutytqb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vvcvfgkm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmjhpxxv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oibptifj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dysycwib.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsyoahzy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zyvvsvdj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jzvjdaei.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jyajkarn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3xtxpwxcn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3npwzijwm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mcmkdhup.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tfheybqu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cmxrzrkp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qyscwlxz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ciypihxn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bhzqeyam.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3zwpbfxqr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3sdkebokr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3drvtdull.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3djhuvugg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3sxbmwlqk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3eljjswcz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3tzywsony.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vacezrfl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3djoxabqm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3vgaygonj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3crpombcp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3tojbwxeq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfsrrale.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3zuotxzpc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dqxqafmk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dqyqagyq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dgxinnso.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zflgwldq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iaskukup.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3kqvueyvo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bxjwqgef.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wmhmgzgy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3whjjlako.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vcodbikw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3gbeipcen.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3egghsgsf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3coygurvc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tbjfhare.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3niavvxez.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dfvqhazb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytfvwtmr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3npxipple.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3huoyszce.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qwacqtfg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgvwcxsx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3usrhctww.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3toueddvc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kfmwqhxs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3tvwhkhyp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fhjdvkur.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3btjcbyun.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3uyjzgskw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yimydpcs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ajseegse.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oowsfdnz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dwjyaxwc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3pehzhjyk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3rmljjbvl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvwjfynu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vmukfaoc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tkrwdmyw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hvgatepj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vwwdprnr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3snrwsxsx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3teskjotj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3iqqmgxja.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qiwtjwjc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3avwcflcv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vikwbiye.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3bdaaizco.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zbbwvpog.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ezxuyisv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnajuapi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzkctbio.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3dordqsve.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3dcjicejr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcscfiid.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3kylzgelw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3aqqstmrv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3onjfamwe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdyoisoa.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xcvhkkxi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aogzqknr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jxtwqijy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3edcosygp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xgmyqqwi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ssuynbda.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zolhxyxr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cxutvprt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hzmrtzst.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3famflwbt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3qmhcmkhl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3fqutjbyp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qwkgdccx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3pyapwdgc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hamstwfh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3jatuicuw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3aqjlkbxc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mhvkvgjz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jbnbjvrr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3uydshpup.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3urawqatw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3prrlfhie.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fanidott.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3trnczvim.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3awovcyqp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3tddexxyx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3fvydlgaf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3mapussfe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ihoocmbl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3kksrphgl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3hvhftwtc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ybcbzsrr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3dexttysz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3khijebiw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3aqaoeawo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3mgjqzjpt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ysjtlaiy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3fwqjxuls.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jndlgeow.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ywfdpvnl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3wiqpjkxv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3cisvmjza.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3bvstsbgj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ooibrxsa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3avmgxrwr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3itdgcnpj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3mqkhbenf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3acaolwyd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3vnwfukqf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3exsmrowz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqzpegju.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3vnolcxmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3airmrmrd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3xrivffjs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qvshbqej.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nmfviopa.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nszwkjil.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3sobqhrmn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3bdfveart.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3frxuxbro.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qleecmjn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fuexwlpv.html


<!-- 参考信息 -->