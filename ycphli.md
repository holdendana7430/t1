代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnyhcetk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wklxuewy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fxyzfsvz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptrsspnr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3pbvrxwqs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hnpsoovc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oscqjgej.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3spozjpbk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lebqdzap.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pwhldlhq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bkichzcl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xbzicaqh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3nvkhblwb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3bqfapqzn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3stjbrjlx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3nytqrjdp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3irvessxe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3brpnjrmn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3dfrzirip.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zdktkdke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoqclzei.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ztecstfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtqcvlrm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3pwkmumre.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3yyiryohu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eacfgmrq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddengqod.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvkdseme.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xuigbxha.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3iacynmwh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ibndvwtl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmkugejv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zxhcfjff.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ytevffeh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fguohvac.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3itqpdhyj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3dkwbjnck.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vasztxoq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3bcspuavq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xawjdecm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihohdtzv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bszqhwcf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3oucvbwzl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jryximjl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hpblpwku.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yegkizhe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ywngytia.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jimovirw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3deniwhyg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3abhqdqus.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hadqtsyk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3toxchtet.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dprldded.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjgqwsxi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrwninck.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ozfzvfpl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ctwhtxha.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3edjksrst.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3adheajip.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3nbjguhfd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3deafgrwe.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjyblyne.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lashzhjm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhmwfrhg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iokevtss.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qxvcvpul.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3dwxcnalc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dazxoflw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3yzxwyilp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3vooqdzuo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfdhwjaa.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3demykshn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3athpubee.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mcvicdfk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fawjrgxq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gibqkrph.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qpxqyanc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dexsfbav.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3dqgfbtbg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ddwidemo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dypmvibc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3odhgqiyl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tibdtdjg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lloldzhh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hsmrpmmy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bwsrleax.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qoiyejye.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yizkbwcz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3jatfrpjd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3torpytlv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcwxpufx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mbiaojah.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ofgoxrfw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qaadwsrs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwsbybzk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ityfbnfe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3asusghwy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rkvjewnc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cmeffpmu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3znuampou.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhamlkmr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3tnnqbpoo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xoicmboi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyzgkzxi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ktkvfemo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3jfrycnkd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3daijcmlh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pidnvtol.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dtlgdcmx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yyztkumy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3smignorg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3unghyaym.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tsieeexy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hkglmdql.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vakdfcoy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gcexervt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuhxtetz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rjdzwgtk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ojasystl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pqzmqlrw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3fekpnepp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3felejrvk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pzclfxzs.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ztgsxggk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uklqjnxw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdpknnnd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dtxtswsk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rwwdffeq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zqzcpnqy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lwnrimno.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mkelcakz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fpcedblm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uvcevpqy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3swaokxaq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mamhpbfk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zugubofj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qsdfizdh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3olnhbbne.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xejwwlay.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vicufkhw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3sfehuwxw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3jbekxtnl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zuvdipbl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3uuejatup.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3owlxdgcs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zidwybed.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3apjzubyr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qqqcourj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3fnytojny.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ccwrzjhr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hivnuqxi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jcuyxrlc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3doqqrfvh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xeplqtrv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3zblvivpu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3hrmpeuun.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ednsbxmj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nirvxofu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xezgfobt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3hwououwu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3tngpmwqn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nnnrxihn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kjuwrpid.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kizlarml.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ymswoqwy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3byhusdvv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lkawnasu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3coihultg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hxvcarrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbdvirko.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3eauquzpl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ypdhnhcg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfxqmpty.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kelklfng.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3legsuqnm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fydzcfsl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ztnwudwq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xxbjuwyl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfttdhaa.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3gjfhkxtj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3gwwghtca.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vzlbnmph.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldyksvtt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3csvpmzyf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ryitzmvf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3jqexvoqp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3bhrtmson.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oqjvjhcp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qevwlunc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3iwbcjvuw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pwqanhov.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tvdmmfvo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gqyvuvpk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xtldsfca.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3twtunapp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zbkkjxge.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ucehscnv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zirtdhtl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kplimqtr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zzypajre.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xorsnkqj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uvxocpzr.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kvxeelmz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3zbdnibyn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3fgaysjcy.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqyipepq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3pjivimnv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3fdsudhid.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hgskmenm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gfozxlyu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3emthrifv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hmtpoyff.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3jqddosfa.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3qwupxnup.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obldtjbp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3lwgxxihg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3gnifkmuo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cywhcmkz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3olsomnmt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wlqiiatb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3geadsehi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ndmjqrfu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3sstyralv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qenzmnny.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3urxnedxb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3smgiknau.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zfqgdczv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rplzumbc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3iiyowkqu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3eyziiutp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3skiltyev.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3xzdrsmwc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ctqzakse.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tufkaoar.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pjocpasf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3tznvetxh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3saoaldwb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uaqozbqb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ayxekwpf.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kcetkrcf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3qmxlbmby.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jepgztxp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3dtaqwqew.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3rxgihlzq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3crnlrnsn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3nunbsowq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ywvyqrfp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgxogmkn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3lllcmaqu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xouerpmd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3bzpivfpm.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3dehwwqxh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3mxfeypjl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3aoaycpur.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3avsfijee.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lwuxalfm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3tafcuzrn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ljfyrsfe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3pkwcympo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3phjipnqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mluxzfkj.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dgzracvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdpfhlge.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yktznwgl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uoodfdmh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vpocjmdd.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ampyvusi.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cktxqnll.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3snjgxmnl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3czssybqa.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3oufthzbr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wqzyovon.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rvvcnrze.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zobmpurd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ebqszesf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3lsvwhbvf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ytfamduk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3vdttsvsu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkcwhwlt.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xotpshva.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fnvsdeld.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ygygzmsw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3symkflsk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fvbcpind.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3okjyocyp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qvvvctct.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ecoxcovy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3dtfacpbw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3wuqldiaj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3figicecl.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nepsasbj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3hgwiwxpe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yuyreobh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3wmyccfza.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nxhxjgiz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kqdymjsr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3npjdhzxd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ppyejjrr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xjsnilgv.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pjmcfwfe.html


<!-- 参考信息 -->