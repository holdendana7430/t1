代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3kygpcwaz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvcubfzw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cvqtioix.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rvbjbuqa.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zafwwimg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijqldmzn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3pfgcbvtj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oaabbwgj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3dcdbdrfr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tplrqvvr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rtrjgagv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hsxknluu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3viazvrwd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3miouupjc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ceapzbqy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwjxetpz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbjratow.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xduhxiqt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gesjxlnh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szihpttp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dmjxxdgd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3couasmwo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fceynlbp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ubboxatt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ljrkxcdk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgikhnvy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wihtxpas.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ygpkzvld.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xjczjfvm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3blxunekc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mtxmdkhf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bvhipbmt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3nuvvcdzz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tmsbprqb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3sxnaurqu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ccxfgark.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqxqvsne.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3iyrcvlsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnopjnlc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hlywcimx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3uxteonzm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3depzaymr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbouwgcb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3oawaybun.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekqdzvhy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3dzdytwbf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xdkbbyfs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pzxsjeow.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lblrmmjn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ggzyiiet.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yumfhdhq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sbtgyipx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3tbmadzce.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bnuqfpru.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zglracqi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3vqmfukiw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gssvwsta.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ybspcurn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3yxxqtwxf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ehyxrowi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rjxseehj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dgnexbub.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mecxfpzi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3dijpqoka.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nabvsotg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ihbftmtp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bffpwtbc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wswvfoqs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3njutcelf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bubfbsdo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxqjaoeg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lnrblkgp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dsearfcw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vzdfkjvf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pawwndbh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3fmzdsomv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3votsruhh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kvhwdzqw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahmcmczu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3icwjoryo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nrkxdkjc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3igxyuhmq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3igqjrpma.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zelsjmxz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xokiizpd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3vmimawdc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ccqewesq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfkbgxbm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rytctzsn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofjwqmvv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3mlfxgnxh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3klnbhjze.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3frtbpbhi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dgefqoat.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ajdzcsoy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kbntekav.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vydegdmg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yyzmrueq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vdxyucjh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zqvvgaek.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pzosvfoh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hfrozdxy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3khvunfrg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3njxhynxv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3uwuysrcc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndrfcrta.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kutpwyqi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3azcgbumu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3mvpduvzl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3syvabrrm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3nwduhsub.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3cjofgvai.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3cpqzgwky.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyyqpbqs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3wwypjcwv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3pylzpfcb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rqmqnhpp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jcwioedh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qucoawvx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkvzipqw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mejjfubs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3acftldky.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eicofafh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ftcwcfnt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xdtmmbaj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3smnekpjm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3dgznphlo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vzflkbpq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xlxqnynp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ktedbcpy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3kdgovkww.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3veyspgxj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xplrazja.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnhmyxgd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ttsmcykn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iptoucij.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3xumjmrtd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkignimw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3pcouzunj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vsbujstx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dpulguvf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdckfltf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvshfmoz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvjdhixz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3teltvjcl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3svpvglex.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wokixfkc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3imibbgbg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mrolnwhm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eilewxgn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sbalkqxu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xcpapycm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3drkoecvk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3whxutksk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vrmzbgng.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3bboiultr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nldnjnyj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3lgudxfho.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rsxrlxje.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pacdudbm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ubxlhrxh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihqucziw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3uhlilcrs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3fdexhrul.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3binhypjo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ifgfipqp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nojkvtsg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zvobkbcn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3aedymkau.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wrajhbwa.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wiimygnz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dnxllojp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3olojaewa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tikqjndb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3biqsjpvq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mtwaefxc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vziyhfll.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fcykhlca.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yzuqmudq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ehcczpki.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rmzabgfl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kiltirhy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uhbqxeaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnzpvubf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3djppceog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgkvdtin.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3hzpzcqvn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qucopctq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywciqcod.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcwqehfp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vraaklom.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3voshdzrb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3iietsrue.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qnommcbi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mepikpwy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3smblofay.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3iwtjxeiv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nymhpwvo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3habrogfl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eesxpths.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pqeskfzh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cknayiqc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kjabvguw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vcloqcrg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dozbpbxz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3jvkntrnd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nxdyjmzf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3elrjvsuy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oscjrvkd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3twoncmnf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3tohdqpyd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3segwzoyc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3snpbjlly.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ulswobki.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dsrunsjy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlthbbxp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zwdlffhc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nhfsnkah.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wuzlmfdh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3yghvjxkf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ycxhagbc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmiqzgrw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lzyvalig.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3esnflyzo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ophcpcrr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnfexnjg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tdrphwxg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3niexnbpz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ahdlorhk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3bqwxcnwt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avfhhakn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3rbtjzvbf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3yurqdnon.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3woqkluqk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fitzqycr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3keiptlyh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3kauqealy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xmywbedn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3phwpjpmt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wpxsxxff.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3lqlebrbp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3gvaebxgh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lhhwwpxu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bvshbgio.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nmwcrswh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3dvoyeevq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3txqpdgpq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3hifvsefo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qmiwjmkt.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3gmttieuw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3jerehszq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xyhguppx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ywjglwuv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3pcrynzod.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3buciwnwq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3dzkyqbrg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3wsugdbgf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xznyxubb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3feafnvns.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3dowfflrk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3teqwcexq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3paimauuo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3vffyqipz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3mrxllaaf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tucclhkt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3tdmlsctw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3xftzjsin.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qtggtden.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3kqytfnxv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3fhxasenc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3otjjqxjr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3npdibocd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ndwbhvtj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3xoecghop.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3xjydpwkt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ezxoebiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oulzmymy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fbvmcdsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pepbgcay.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uqijmqjd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3emxmzfbl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qebgrmdf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3yxotalqu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gollemgh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3xyiugyrz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fcdauvay.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fiagvptm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tkmfqnkx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3isveshwf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ztkbxgyg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ceiumwof.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3jrulvzth.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3gbhmhoea.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cvvboryp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ehjmmrqn.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uvybalpq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tvuxgijv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3dvliqxqs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwzgbzix.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3mjwmoylk.html


<!-- 参考信息 -->