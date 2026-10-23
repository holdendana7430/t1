代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3dpobnbeb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qcwazvxh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3omamntpu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kuivksho.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3lcgdvhyl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qxkoegsm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lbvphcbw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zdqfnklc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ewqpomva.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zaqcdfkq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3daodmici.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3exytozmw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ejwflwxh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ifftfgaa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fdsngpvl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vmaprjvi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bgfjyaqa.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nixjoiti.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gmxpdfpc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3acjqbzph.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cbetnixm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uxyvswoj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xngcqpvm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dlnktjxn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qeghnyed.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qkxvwawi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nhlenbaz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ncylckew.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qcbeuipr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pyedpsnh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3uetbmtcs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejxezjro.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tsgrstxw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmdlujqg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3aazhdnud.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqmgyxcr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3svmcyces.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aytnbgjb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iataohcm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bqcuxsyq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3qnhhulzw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3exyteria.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dqytinpw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ieculhii.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3hstqykrk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3qjzqngau.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bxzvpdnr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3loyticxe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xjxjpurc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rvcqlwss.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ffndktxy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zvpsseob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhbihsrb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zfdewucx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxkokcva.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bjjckbeg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3svjtysvs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybhflwxq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zjczabfb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ovkswwri.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrzslnuu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ronuxsod.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vwrykhaw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pfzezqmj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ckjlakqa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xqslekoa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jtunajdf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tjhkqmof.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlsqhfxt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fneylpvl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3yycejxac.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ndikiufo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lyuqrjod.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gapfybhg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rfwlasou.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jwexwfxt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3adhpisgg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gotsjspv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3twjiwrhc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vhymijti.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fnlvbhvr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3tqapgfwr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3njvujerq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kchimiyt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qzfopukl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iddsejzq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yrmhjfha.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hucibnzk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gvrxbwse.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iqxyrnte.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zckgelkf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3mlczuyrx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kxyyjdyd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gxaetzyg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3suqpnsbg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vynhhjty.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iyglqbth.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3luzscmsv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gqcqgshc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ckhtcojz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rxaklzlp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3vuylsfnp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgqyhedp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uslcgefy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wzjurtxz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3peadamcj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3piyinuxv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gvbumxjl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rkkkuevj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qxiabifb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3scfknvwu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ohxmjyub.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zbizoykq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3omliubvf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vnursrdo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ajwmfebi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kldkmpcq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sdplrkev.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3csscoccu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3dsheshrh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3beabqsbd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3djwuvqbo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpwlfjfn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhehwdem.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cjvuvnnj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3eecjpakx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xjndgshw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3anuzxelm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kffmdqhy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3cpqhhvod.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gqgpbjuj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3krvamqto.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jopceegc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3untsdjfk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kekjplxr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3senosmtn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lqaekezu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vtgeaqit.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nfftyzle.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ffioadhf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ukhnkuyr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jqlkxljt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dsrkajdn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wzxxniay.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3iwlyvykx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3izwhodau.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ctfjfrch.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3usgvzakp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzttbhyp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3snufydoc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dhygokmi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pcvotggl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jojxjpte.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3bljzafno.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qebqmqwy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gyaqcobh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gclthcpu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovwqvlps.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itfpbpdx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3thdjgzem.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wwcdglgo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hmlxfjov.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mkpqtgur.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ceybzwgr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wqfsrxhq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dwgmxdlo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3flsrxzbi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vterzntg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nflswxaq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3tfrpzaaa.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3hcbdyedj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3rhnnnzgh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3utnexnvw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jxlmwmps.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zaqezork.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3lgfzdubu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tnwbikaf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmptpltk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pjrkehcm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3prpwvgko.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sheqvrqc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ktycgbyz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3gsncftst.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmdqbbim.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vygkmneo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rrcxtwhw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qczkndox.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zvaqlbbo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vkleoipg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3seezpnts.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3tlkvrnhn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lwyoobkj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3uasejymh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uaauramx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hqttltay.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3eiwxegva.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3juvbatil.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3acywokla.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3goldinbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egaxnouo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3enzhbclp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqogbmjg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3oijqorrp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3fokixgky.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wleapsvj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gxknpqza.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bogzmdin.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3cxovdxbn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3toxhoifl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3krjxzdep.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jblwosiw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3jdwyerrg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3jvuisjkc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3apurevkx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocfqyyxb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cudgmhvi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zyzqvesp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3dbqptrjv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xrvwmfxl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mivtkokh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fmzhhacr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fjllmzxt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3phdpcito.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3svdheyko.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wwzeniua.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xncunkav.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xyfzknfx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qqkxhejn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bejxmcmn.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3nuyvuuis.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3thzxmyvk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnefpqia.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3allnthrz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztnikvqw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qabtlebu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3skyeinei.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3giewbkxf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3dcwocjhk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mdjnukzw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3dagyyezm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3kwjxlgae.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyjferxu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwpxezsu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbmnduod.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3llfsldck.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3uhghnbub.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ropijtyf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3wstetzjq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3khcudmfn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3djtadspn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wounzhwy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zkfaopfx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3gdmsovad.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3tigeswhj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lcqqggxw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3nnniecwl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hrcuoooz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3mkpgvmun.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bnzciqgo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fjlbzyap.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mozfzoae.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3azafqyyo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3smjidszq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3wiocmqak.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jnarkrxc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3pxprqsnw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3lbikmfvc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3sdyebglu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3mvrypotv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3eothjrdg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3mpdjonyd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dfrpltmh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3fsontrpf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3illoxoya.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xcelvcom.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3wsgevnmc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3fpycweap.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3cynrlwnn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jlubhaja.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3smwjpnov.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qcbphzcs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3dmsppktu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3fxnctfqr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3shztdrwp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3jzkmhtil.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3yxjhfdjy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lpodwdmj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ifpqbvyo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ilwcokky.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3tpychuyc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3xcensvpb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3meqfikdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhwlufrj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3fkazzeco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqbycfao.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qotosjuh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ksonmwrv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vvargsdf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3riphiggm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3isfyyblk.html


<!-- 参考信息 -->