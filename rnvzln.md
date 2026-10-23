代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fuhwhsox.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zezppytu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dcvmpqjr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rsyvouuy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zmbiupzl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3njpyllbx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ihfeopkj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qbjqfflc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rhpaivkn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gipwpbrr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3egwqolym.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzlnqprt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3detojtsb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3vuktdmwm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tefzhfor.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yvbdgpqc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rheoseyi.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohtejytq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dbxzjihc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3acsigimg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nexipsxf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tahwbtgy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fawokgbc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsmjlhln.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hqezimie.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azrrydeb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jhnnhjwc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3avjlhdoz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xfpoytuo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ahhiaczw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ygnpbkkh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ghxcljyn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ecsprjhv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vgqndmoz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3kmowaljb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bgsqlrhw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zdnvmcez.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rnggqwpm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3npiyjzxy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ntcytrbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjhheynv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3klixzcrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjrnypie.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bnciqwvl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3iounxlnf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxzlxqjp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qsqhrpvq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3whsdrvfo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fszwrgma.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3cogjhhpx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3efeipckv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qvvgohsw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3subntslc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wtzlhmcu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmxprtwr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnourzfz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3whumaems.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrafctdb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ymghozwu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3efxvgtbv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grmrabpf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vajgeyom.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gxljamfs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gveqqjha.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vulwtiiz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lmytlbvs.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hqroclkk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zeluocxd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xhnaghqa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ohlrddvf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vmxgxbgw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pfobycbt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yytauvzo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vnhadaka.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3opmpawan.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3geqlwraa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lwqyioim.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3eridgsxq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jegrvafg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ahvoyazx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tgauwmeh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ctsqvfas.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3phzvwtyo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxgipbef.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bpnkhjnz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bfkgkciz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lbvqjdbs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3muwynjxs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ntfbfnkx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3adahcvxs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rsoqqtgw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmubjkyf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nwisqxha.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbncxvfb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3dewftmap.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3eqzflyzs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tobciduq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3sgdzhowj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3tqdeisav.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3upjozgtm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pbgwojtx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nogdbkqd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fbfvuqnn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pfosunlu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bgoqqpmq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lceuqlll.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ezfvacxr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xdifqldq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnespdis.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3htrekbmt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgygsxfc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3exusunml.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zaxgzhxz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ekxncoyu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3cbtgtuhz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3hpbbubhd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ghrnfytw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nrckynth.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3vaocpsou.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mewhzbbk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zkoqsjgw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3djyyuyzq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ozskgncd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvikzzst.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3thxqebqc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hntimhwr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ldqlkwgp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3wsdyrggh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bgteeyal.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3yplsfgpi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ieufuemq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3thjqjwxr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3icdjxygq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mfwtyzyz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3haqtddyx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mnhxhyuj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pjqgkxqg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iytxohyd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pfcpfffd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3preeopas.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vtfyqdhd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3zofoalso.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3flamhwoh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3momhqimp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvhmmswb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xugdpibs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3euplzrrx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ssfvztvb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wgpctktw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rybbajcd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ighlhslt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cfqwwwml.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dihnhech.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lqdjdrmt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rscziwfb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3npuccnfo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cqqilgao.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3xxuknezo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3foarhinb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dwjoycsz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zeleuazc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3jcrkhpqt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3uifxlmgf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3cnxeduzz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3fcpwlisw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqzkdfla.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3xchfqpjq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qfgmjqct.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3nxrnfjtg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3psevyhhq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3poimjvge.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnorhhka.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3aefrmxoq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3enmidfjb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3quhatckm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3bvlkcqro.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3wdhihnwn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hsdfkixo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xvpwnjrq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3uafwrbvd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vpgbivyg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dvbucwzb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zavtyhfp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3eyltidic.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3cfnhirjl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pxcvfqvd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3oeptolrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kynesgwr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3aiwhvhcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuqhhiio.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rsawqlcc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3itnmyapw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3oyrjtsrx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ndrgsjda.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3isrzsmmd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3naudoklv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qqcwbsfk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3rhcvlrla.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wonkrwcz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kktxucpn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3rhejcdcb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3shcpssdh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nfhsmely.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtbjnllb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfwrcsvt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ydtsjjie.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3phumzmch.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3clhignjd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rkphqrrd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3haabxful.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3odjrypji.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mwwurdai.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mhvipmcy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ujnxmfrn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fvkwinyu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3vycfvnxn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3siqaeodg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3bcqzvmzb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3oujnesli.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zefjkkbw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouaimqqv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3esljncpv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ohyndaod.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3iavycgke.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rkifgoru.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hfuzyzcz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3pgqcwbkt.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3rvpdstat.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3misrxylg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwyjzvra.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3seggpxmd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hgxfmkrs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3wlygjopw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3stdnnsdv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahceilvv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3dmkhfmxb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3idhjizaw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gchvdjgb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3prbfpevw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zzvscseo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ntrylqsh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ldtryhlk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jrakrhrx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fdaivcca.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3stzuakii.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3tydluiem.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tnblctlg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oigqurck.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xnvizylg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3guerhbzu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bccobujp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3hsolmsql.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pbnlxhmy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3wrnkfaro.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3nnfkcjhn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ixhhogkh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3jpesnztf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3evbxqrze.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3gpoxwgey.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bmtfuqhk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3chgsjjip.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ahjyxywg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3qersysbe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3lszhpmtn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ugybsatu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3meobttjr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3lussgeah.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ampsedgt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xlhqxbby.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3kwicsaeg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3vagweyha.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3fewzxrzd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pheyxwkn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3akzvvwug.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3euiiveot.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fcdjvpja.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3hcsqtdfy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3luagjvxz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3qbotoatr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lflwjxmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcqlckoo.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3xssvsiql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnybysol.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3rlyfcvpt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ypvcmiwk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jdeehojj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tdpyfmjb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sslfrcfp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3dxlmotuw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckotkdei.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3vfsoasud.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3duwjrrko.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3xmucxjnh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3tflpthsr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3rwvxdixs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3zzctevhw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bpmjnxxb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3zgowvwsw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhlckikm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3niqwfvwf.html


<!-- 参考信息 -->