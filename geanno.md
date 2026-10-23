代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hpffwliz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itgfnoqs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jbdmdfik.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewjeffbs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mddyxcih.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qygwjpmt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3znuwndjj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cpznyjpr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pipcahqi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjneitsp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3onukvgio.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3jbbjotdx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cbrfvwqy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3qxudwyqj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3dophttes.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3dgnkevgc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zvccitbf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3eoxrdatp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3voccchup.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rlpmffzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3caopqhln.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fdjdndgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgoseipx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3utjzvbtn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xhsqzmkh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mheqmpyz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfbjsfmj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ocltlbob.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dsyumfzp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3atvkyrvl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tafrhjob.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sqfnjawp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zdphfwcx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mpwuuspx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yrkyhdvb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxogeuug.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3wrwydxvo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqpzeame.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3faxqeide.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3szcxupgd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwvxkbbn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pddghewg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qmbxrfsz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dzlslara.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dfnnidzf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3icbpabmc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bddsezzp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hmcrktsr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dosaepno.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3kmzariei.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lcapyhpb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3efbqypig.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mwewqgbq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkxwkcts.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sifqbvxg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3csbtgmot.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3phcadepu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qlqqgukb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zrlxwjbz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gnttlpjv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3pmbgbcau.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3areaywhl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oubwadag.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgbxlfay.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhwcfmyk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3pwpodpst.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3uujmnylq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbwurwbm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xwgladyo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tsbehbrm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjfrrvzv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozdhqept.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mvrjfzrr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwjegbwg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gbatdzjw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vleqyuqp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qqkuxmhb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3cajqifni.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rymwclrr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pojqtmwb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dfmpimds.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aglfmmdp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kexxjnun.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pjgfprjd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3btlzrvwy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3soxfstog.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ixquebix.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wjaxowgv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3naoemzty.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbuhogzn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3iyovrohf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rdsuyblb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3lsrzbnfo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3vzvjrxzn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3biljehrz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3iybvdakb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3aryyhuah.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3fjafzxlp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rxvslzik.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3grerepvv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3frljdjhg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3khyeesnz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wwmaycqx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hzwxnuvf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ndovsopm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qjjnplqf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ytqkpchg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kykgipll.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eduowcmo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3dfjaxazb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ilthrdhv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lnohbzoj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tbralmev.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3nefurdjv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3litowvzy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcuzgwoj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zuszjawa.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxzfdsyh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsunxiub.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iisojjuh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zsdslfjw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3snhkkmjg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ozwfjuyp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3swofsbih.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3viaigaow.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ejklwnhy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbhlflnu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qggstecx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fvgkmpyk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ludkgizf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kdkwspnb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jynawyhd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lifxqoke.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3acqolsgk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qychfolm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eeydbpdq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rfcxhqms.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3gldnhpqw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lrlioxul.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tzwxvjjz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ujorctzj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zaposbef.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fwsveqqv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wltekoac.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3aunkhlwa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vbednafg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3omofgukc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3owdhigui.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mdnlpsve.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nlijjhbb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3idqgkaqu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kmeweeqo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3pgvnqtfe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqemelri.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3niwsozbv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3fyrlttry.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3iosstgjj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rlqsbwuh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xmquuqlv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3sytnkhrh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vkqlxwsk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ujydrsru.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mgjskhyt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mqmuwcde.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ypcyfbrr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3tekaqpei.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qdivojwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yiivlnon.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rgxhbeyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3doqdsfaw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yaqkuigi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgfqffc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3kdlsgdeq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3angbkfkb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pojnitlw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3frxmalsu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ufoeteqb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3skasicpc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwqmqdax.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3vnxscyzf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3himzirtc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvcinjhn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3adkngufc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ljursgrm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dzxhwark.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3gvvhmkpw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3yaqsynxv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkuohcqs.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lbhgktgg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3onckzlmy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yfzqwvnf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ubssggdf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zjnkywnb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hoitgqmr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3eglodoug.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ezxdhnlt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vphldfbp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ahlbshzm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hznitmai.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vzbqodsy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3sxddbclu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wouqpjoz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tlopgxca.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3qflshogh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3huwyimmz.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3umgkkppe.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ypipefsh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ydhwbdoi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3egoyeqrv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxnnnlpk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ybzufxla.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmaxcdbd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ugtpikvm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3imljjwch.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dklssgiw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3rnbtkoya.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3edeubkgb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zojkzlgn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3axwhpalh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3urotqhxj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ipctlrld.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3dycqzuey.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qjryaqvw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3afcubnht.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qjugzhex.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3tpihzyah.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ejurefmc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kfyxzwnz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ensmlarf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ccrdkmex.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3tfwkwxts.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3sjsruacu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ppaubrhl.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3acrpkmdh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3psvlcrhm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rrjurcyf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ozxndmup.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3cwkmvtno.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3aduatmeu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3jizypkqp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ayzvhjod.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3wneotmax.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3bevbmxtg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3atvwyhup.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3cvrxbzgt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3zuuoijrh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3lvnbdhqu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3uglyqnmi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wdexcqmc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3cbrmorti.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3kdogdzis.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3taktdvmq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3bademwpl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3jxybkqmy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ohsmpboe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pvdofwql.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3isbivswx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3urmldxrq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3thgonwht.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vbghtzkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqoqzpzn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fbuhjnfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxitnoqt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3revcfvdw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3myxycrid.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jqfmmypr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ohllnuon.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxoykptv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rkkjtzqo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tthufrip.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bjeupqhd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lkufpceb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cqpcfwoi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewlixgdk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wqdcfbjo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3bguudtwu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hnykfmfw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3knqjcvrj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lnntjnlx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3egrkorwl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uzbwyiqp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3lfzonybz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3bdzgizrq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tjxmcuri.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lkumzonb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kkmuojqj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3yizffwgr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3wkdwhksv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vdexhsda.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3uymsomim.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3eydifjbo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3umlhajkf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3teoitckf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3oqjofgrr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3blzcpsry.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dvisiczq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vtscivfw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vtgswdsg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xxnrcocf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zyofeiuu.html


<!-- 参考信息 -->