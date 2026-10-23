代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qldpxgvw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pipqzskq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wnyztfvg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pxmvjdvz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gnmbiaqx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ypdxjxwz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrrwcmar.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wqcueuwj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrnlhmql.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3shykdmeo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3dogprpyc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjhppkst.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3djykmcai.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bddnxlnl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jinfergp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3efwxwfbt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rlcnesmf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwwxqrjy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iyecbalr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nnvgfnbo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ydziebmh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tghnbmuf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3vvczpbkx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qohhrjqp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3hgxdoogh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kiwwpkeo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3iwrrnyti.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3dwsfdnmu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ueipxmcu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3lvkewkjm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jemfawjr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zekuakjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhbbhmnh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3stxsnmed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhtfhoro.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bkarvxoq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ycghdqrd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3teccqktp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3poceqkgk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nibvukmn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3avwzmoxz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rwdbrvks.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ijgxscml.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3skpsqnfc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yxubjqsd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nioiswhz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dzbcluho.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivmoxaim.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3nxkmohun.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hhglrcfj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qarrrrfn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qijqghwm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lavlwglj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3agmwubbf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3twpbndvx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hwfwidda.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3isdamlon.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3twyurahn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nhtwlpyg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3npsqowue.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mvpjkdze.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wpvcytfy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xfkwrceb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qiotmxsk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxoetbxv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eiqyqpie.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yrlbrjen.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sxyxyfgj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3avpgdwqv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kwmzxznl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ycduhzks.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dgmnnzmy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xvixnzyp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bclbrpdl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbqdsorg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgfbcopg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ybkzkwee.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mvlqbvop.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qlbqhilz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vbcwphtz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3inmkprsj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hsjgytxw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiczhvbc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ckrxdfdf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iknkgbfa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovpyfens.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vgcwzdak.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zyjaqxhs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gvoenbzq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3owhgyxxv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bckxyvad.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3icinriya.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3obchxepp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3skqjolrp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jhuqxuxu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3euknrxcl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yftveaen.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xmqrmzjd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mfexgoux.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wkdfxgme.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ftkoleiu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vvmtcpbt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3twtrsbpe.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ghdsezyy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vwhwwehh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3isgqxdik.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3lkqecafe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3udwzuang.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3omyawjmi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nzmboyqp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dnzriufd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3krhxnnph.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyptarsu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kaeivqrg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ewzdbbkg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tyjxnxmv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wuqwkjwl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bbkvklbk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fsdxfipq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hijlbtxu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pmfyznqu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jglxdfgy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cbmkhkjf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vyinmwab.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vsvhisgb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jxvkjfyx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3wyrukgax.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3egsenkll.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqrfbgrp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rkxhjdul.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tfjksyzl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ewroaxva.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3eoiowdzb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhcsbeah.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fxfkcphe.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3aajtrvzu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkhidhpo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3djqfmgcx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jwajipek.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mnzjwrbr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yfsxqgmb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rnqtkqex.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sjddpkhj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3kqitblmh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dymvasrz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ftpiluft.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zclqmtgw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yitrhefv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cyidoedv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ftixxmvr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3nyrohwwi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3nsaaunrf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3apvajihu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3tbnibysp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zyysxtir.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pwxzowzu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wmdramsy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxlxlvnx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3urxolbct.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ycngfxxv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3uumduojq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pwikzvcl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zvuyiluk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xthqdmgo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3urrgvins.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hmkwrmhl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3trmvvikn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3cqfacqnk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3gyxvsbse.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sugqnllj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ovauwrsx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jsguakoa.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3jwzzncvw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3asvqnrnl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tvojwhdk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jgzjxzel.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vggqvuwu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qpylkxgs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3uwnqwpen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztyukjsw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rcqjruqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xznqbwms.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3nfpqbotx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dtoojapv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3tphhggtb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmwpgeyu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kumhohng.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3tjfpzbfl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lwrwtftk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3znxflwnf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3twgucvbz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rtvotnxo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ecvbbntm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uijhqdvo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3impjwklh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hppinext.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qwntzfll.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3vukyffun.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tujymqvi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldlpbmku.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3sthyirxz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3abgcunlb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uobxlhrg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mqkvcgnq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ddepwknv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gcaumhpq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3lrqqeicf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qdzepcgi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3twxowwmq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xlbrjnbf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dqzhsxzz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rtlpqmeg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxxkcwty.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3iyxtkdrf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kejgrmjp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wnwigqvu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3mnsczilw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3mygutqsl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mjvgeqlr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3cmgowctv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3gyiyhqbx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bqetjzmb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqezlood.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3gnnkuxfv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zcjsiakv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3otxrsptv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxqrlrvz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3wsezaert.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ktmwgnsm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pfcbqikz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hoieophl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yywqitcc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ijrrciiq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xogqwbih.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3auynpasr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jrmlhcfu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hwmjmvsw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ddzjsbei.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3genegrpt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3khycfkvo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zhgmtyhs.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3wrupkfmr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3sbejwvwf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3wsrkcver.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mkixnxnr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3eyyqseko.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3dtyajwey.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3lfmzzrec.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wyemklpq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zfjstxbh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3qebffgrh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3btuuetsf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ymnfzfhw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ictqofil.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3nqluxxdt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3brhzgbae.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ozzypokc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3jiyhguks.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3bhzmwgru.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwyznhbi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ttgtydbg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zulvbwgh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3rgaqwkln.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3odhmfxuz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3mwzwdhkk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3togvzdvm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3yrzvkuzv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lhbxpypt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ncrbjlpr.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3bajznibi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3xywbfmkh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hqbijemg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acecppew.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3siclfjbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqypfequ.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3dfzxutzi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nrwlcpfc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3svxdriqd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3igcjgdzk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajaulgcg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3aqdbokpf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3asghzjrl.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3najpzzcr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3scvwitub.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ypflyzxy.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jycbclgm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3hbpfrkvb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3yfwiwsmy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3cudyjwiu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tegctmac.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zyqjxott.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mjzccefq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fnslgwhb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3pfwydubx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3xfakdpjg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3eztqdynp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3wrctusax.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qgiinyit.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ocaegexq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ozcenpdy.html


<!-- 参考信息 -->