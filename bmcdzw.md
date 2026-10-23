代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dtjokhrw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhfffqje.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iteutktw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xwdjlwsd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pviwqsqa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mimujkop.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zcbaojkl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gtyjejiw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dsskbreh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zvbovaev.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rdzhiusr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fqtevxai.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3swxknoqw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ijxlxflt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ehrjfpih.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3etzsdfvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gazypjvh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ofovfxpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnmaubmq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3sppjusqp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3shmbktjn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3avwazcwy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyambwqv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygbbxwby.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qhjstzaa.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qsxnqyom.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vuezrvjl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hsnjmbda.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wngazywz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xkbcufea.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mydgndzp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ptonbdsk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqwuyyfc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocxmfjyr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3lsipnoyy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wsrxvgdb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjlocuyz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vxtvbqov.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ctzhfowg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lwallnzz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3igcmyjod.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tlytxjcv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3szfiwozk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zhcfyteu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kyhsvszl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pychmbvc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ipmcvcbe.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rvwirhlu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3luhrjeap.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmlltyhn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lilglinv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jhpxjogv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oiaejveg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vrigbalc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3htqepcdd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kbiaoslg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xjkexoxf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3faggyahd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yswapkez.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zstrsxee.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mgghpsyh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3wsvntmbj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3innmnbwl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wuhscsbh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3tciuairw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ptkmgzbh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3plhuhycr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3encqvuhh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sdlxfpgm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gfdjmfui.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ensamxyn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ohvvjbol.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3krpdpxyz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3cqinljtx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gxfoagah.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3avkqjkyv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ssswsgzz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ergrsbsx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3holoxdot.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fhidbhjf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jeauhgmp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lwjkmhdo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hasrngwj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wupaucgm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzhrohvr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqhmibil.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3torlltys.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3fihlzqgs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ckwpntgm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lcpsqqsb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3utotktwo.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3enhnabpj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zspsuvmb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ycfrwudv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3uayyriqe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3aujyjijz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3onwwjyqb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3nqxnisup.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tqqrrzyo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3lnzaedhq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3aetxqmdy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3gpcokbgv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3aolpfzqz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3sozcggab.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dqsxutrr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wywhilii.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xanelljg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pznyadud.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fubffakf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3glmvkctw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3vekfmikz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xczqvwhs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ulmqdfco.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rowaodiv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvsbdoqe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lbhxxhvp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cbyebdxt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnmgncrx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ebtuddqg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jqrsrrdn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3imtzmxse.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fktpmswp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jvmgisma.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lygdyktl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vvowibth.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xryogifa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ijbubkbi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ofgroivx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xgeabvpn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rjtujwcs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zdcckcjv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3njjfrsjp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lqdftobj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hxqrcrxr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ixhbwrxq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wafsjolz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xgpnwvvk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xomaxvti.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3wpxhjins.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3irjqquay.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3dxjnbgeh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujphlcck.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hqrmdqkp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wwkjlbhk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tpjavnmo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ryerisvl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ltptmcwy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kgotyrtv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dwaeaqto.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tjjchggr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3pumdunuo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ilnirkch.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ebavsvgy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jgybsdtx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gmqrktot.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ksypfqqd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3tevfotus.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vbqsxpjd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3swhlwwkk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3adujbqws.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rxjjrepv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ycggxphe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yzxmsfcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imzifsil.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3deltwadn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpjwlhlj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3xozguxej.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3znyebckl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3osqvwgmf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3awtwdqft.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcfaoofh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftlprmtm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3yujavswl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ybzztiua.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3slidrwzm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qkajfsen.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3uuimmhow.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3emrmndei.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3stcnqzbn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vygspqgz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gawmjqvw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3gnqffrrn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3jbtqxpil.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwxtwhoq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ptqndfnj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3snhwkzns.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jxtsjreh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ytvwemyd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rtusgbgs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jnfbwlkn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gznanvxw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ektvatzw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ttnxpadq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cmsibhev.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3loimabor.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3punxetti.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ncggvfbb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kneoiodz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3acilcsos.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3axsddmfa.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3devmbllm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zamyvati.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ijzyhntu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wtocjaxe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3okhnvwwy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rqgtfijb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmoeuean.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikvpqjiu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3xiahgdzz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xqqcxfwb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jsmrmdsk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3myfevlzw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hxowkuos.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mxzidusw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kvuzxiua.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kdfogsqj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3gfehlkaz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vtsfgtxa.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rgdbubaw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zgkxjzmg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3kmvmcptw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3tpritune.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3myiinzzh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fsddbtqe.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mjmzokaw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3mlyxwsap.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ipmtpdjl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3tzywxihf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lextfnyw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3wjjxtsby.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hzykwxci.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3smtldfbs.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3jqwnuvzz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uttniyay.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hgpckadf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3fcvauuao.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3zmvjqfca.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3nshqinyu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3tevbadop.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3osipagjj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3blajbmze.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3uqbwmurj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3wuqgcmki.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygosdvgr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3pambpodi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3fffyfpee.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3imdnaaaq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3maukzpgm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3heacmrne.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3lzjehvum.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ksszfncx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ydtbdder.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ovlnpbrr.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3vvvyqcnq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3biruwsra.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ardvstsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdeminlx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3bihpmwya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttspilmw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3hvvsdofe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ltgelggb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3knssnyrh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgqanqxr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3bespomhi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3byysdspu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3uccbonvl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3smjiiyae.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nllwmocd.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eqjaityx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gtazkorl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3dqincgwf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3yaxqsfja.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3lriwzith.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3besenglo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3eaqdyilw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3igcvantz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ncewkshe.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3otcjnxbo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufuzgmhg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3khfnhrdc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nidowxyw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xrcakpzy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ukxoaavk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3hcptfyld.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3becsgpwi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3cboguvua.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tlpwyfjz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhdhgsun.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vnypukbi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mqqhxsnc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kjosqpfv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3eivpsgae.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hndpsjfd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3qoshiwag.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xoarkhrq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3meuiynmc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3pkujvnsi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvznqphc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3htazvdpb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3efckswmu.html


<!-- 参考信息 -->