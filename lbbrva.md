代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gzybnnpv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dicgosba.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rvvdxwpw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vvpmpqak.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lrjbdcjg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ymwyribi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thvklffw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jzvyaoqk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mfuqggbx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqfrtdpe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mcoqbcez.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjkqrrbb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3plbuezlo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3icaenvgh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qhlwcpzz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlnkaiji.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hfwslphs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qprmhuyw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ecfinjrp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jxqwhiba.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3mspgfmgs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqtdbwou.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3astxomoy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3irlqdkpd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ofbknagw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jehytkhv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3aqvbfqqt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ihzuswwq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3roescmqr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3homfzuee.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jdmaofgz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3occoesvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzujuuru.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3igixqryb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zeyyuswu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qyctiaqo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ajsxpobp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3khticitc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zmhpjohx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoiglufn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fbymglye.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vtwddwdf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3brbvropj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fnrbkgqm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3nhyirxzo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qjtdodwj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rriwecjc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3adbwxrkh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgobytnu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3peeextnl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bbrklrbp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3rmexvoqv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cohzdpbq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3mlaxagbl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vxfwdbys.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zsyhmwto.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qpyygzyl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3axyjoint.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ftxvsccj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hzlbozzj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vrwqziwc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xpyzmjby.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gxftoihl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3aepxgpns.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ossolwoq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfihpmbm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pybxclmn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xmyeppvb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lmomfkau.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qohznoos.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qrfcomiq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zzaybqvt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3sjinulxe.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wpbabufr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbemfobz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zohfvcvv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihnrmxkw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gcvkfrwk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qtbfvrff.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3sbscfmnx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3uvoljyvd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3leefbabo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tyhbarte.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3htylybjx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkhnkqgj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ocuyjcju.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3sbozeeyj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3getxcnoc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3mdylnezz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rptseqiw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3mucctnqv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lmgdfonz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wxoayxkp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kqbeqrsv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pscrnfyd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fomrbtea.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wlomwpsy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wbubhuhz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3aclyambh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3caqoyguc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wbbjdbmz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3aukhbtyo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgjoyzrz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3budlqaiu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ohkqhizi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ewfiaeko.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xftgexom.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ruzdufqr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3nmezfifp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbbuquhz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3soyaeecf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhckxxka.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3akviqpgs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jyyoccnu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hqglueif.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lioliekr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yufoexpp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3yluawjja.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hyiakqsa.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3grxrhyph.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3otncsbqq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3liesosdv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3tozaoszc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3skylrhpn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zzejxthi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hdtsxvwj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dmjpwqca.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltzljxja.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjogelgv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqhwzlzb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dnecvfcv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gcfhlxrv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3snnndjjt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxehmniv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ixruwokg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3urxvoiak.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3huulrdtl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tbhfjtee.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssjdeqph.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mgjflwyb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hzjprpcx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lmuiliul.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fdaozkot.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3xxrpkdby.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mksaydaa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gdotkqiu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pliyhwoq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pfuutcgr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xrjerwuj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3eyeqnvss.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kmljcoid.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fbywvjha.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jenlxetq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3axtsksdy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3sdojjzjm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3aznlqmyf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3iturjqzm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qoxmmrsj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3aramocke.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3oqvgvlwl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qjplislj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3udhwncfg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cavbtiqr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ybozjzii.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qsxwheyq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3llhmsxpq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fxnarzmg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ritgegaj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3cnauftoc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lfvxwkbx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3flkhxfwp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ywbppyki.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ijvmouab.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3obzkxvdb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aazolgll.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3tldptwnk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3oddtljbn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dzrfnqyq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3psmzfttx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqvljdsn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ngwstqnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufgsjqjt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ptnmbwcb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nxgowakz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3luouynuh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ebclcguu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3omncigjw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdtxhlqp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3uwxotmoi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jkqcrvuk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkcndrvu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fxlspqmn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wrbglsxs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3veqstzhw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lapakrut.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3minutlkd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3imfheltv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mgbkpahs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dlyoezva.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3neqqklch.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3edteooqr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3qwkyddvk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rffvlirv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jsuzcqfs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jixaqmzu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hmuclksd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3spmbwuvd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3mfjelrpv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qvyvrtks.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3tclyfrep.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xqwczqzh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xmihmwqv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3srjthfqo.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uvlndthb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wklivfqb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ewkeonnj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3cklywlnb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3cihuqopb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3swbjctbi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3cwypyxba.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3fzqrdtow.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yzengpij.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tauomngg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3dktyhxqe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3nrfnlgvb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3iizxehot.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sukzprat.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3krlqwxcc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zaxglbna.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yzbkyutl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uxyhywhl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rssaylht.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3dmkpxzii.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3rautghjp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3krzwbfer.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3gxjhaqwl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3blnzdypx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3zaufygki.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rawevnjs.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3krsbwjff.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jptmgpos.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ciirftgy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hulxlkqu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3knuvzgpe.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qoreiksw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3jctgqjgw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ysldonlz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xaulnync.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3pivxibsp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3eeuhtamf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3aggahfih.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ujyynyjz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3rpagtwnq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3oxofxnbc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3nvscmtip.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3jsxplfnq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3pgqihbfl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3hsdkusmk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3hxcpoopt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihpdbwql.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3srgasxhi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3fmlujlia.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3kuvwtzqf.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3pvkthvis.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3lhyinmtf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3dmelpjbb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lmudlxey.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3peuevdae.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3euroylsh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3oijokute.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3mgrentef.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gtlsgrxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3taejudgm.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jyatiddn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcwltynu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xfuhobkw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pydqmqnm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cczbuxna.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3enbzylpk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oakodgwj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3nhvymviw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3bilbmjac.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qqyqbhes.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ssvfvakt.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ewxghztq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3cplvfkpi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3azujmdmg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3zdqjwusb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3yqwyevyu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ieukjjcc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rodiyyzh.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3yzjhmmit.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iyaghbzl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3qxthlrpp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3knimrzzq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3smelcjmp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3vscfuahw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3qvcqkqhy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zmfvnjaf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3sxoyxqpj.html


<!-- 参考信息 -->