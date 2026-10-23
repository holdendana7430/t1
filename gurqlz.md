代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jrofdneq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzylftfb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3sajirxci.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3imexxnsd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3edykftyr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lnasauot.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ikfzcffg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ubjxvfmp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3epsptzjh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xwecswrt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ysdujwjw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mfmfdlns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpibypzx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3boicceax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hemowbhv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jhvkjgrr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wgmfgppr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3scnqnkzp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rfqjhizz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ldmdztwp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3loxuljac.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3mhjlqgpi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zrxoohxr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nizbftcr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qyvslphq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3iywpxfgv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unmicsiv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eetfibpu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rjerzvle.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkfggkha.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dbpmnlpi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dxbtghnm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3enqdkvlp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hfslwyyh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3swtsjfcm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qxksvziy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rybhlmqt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bissdkwb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3sfqfsndz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3swwfajjt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dwulmquz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3emmmpouk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gzclafds.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pijszdeu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kmjgmozj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fbbqrfeb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqgghxyo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cwipdasc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zhvelglj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ffooivco.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3senxfjrj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gxizmqnh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ywrnlwwj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhteyclr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3erbeozqp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wxaobdoq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpftcsmn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gkhvguhe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3obsqxzob.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfdlgvtx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ceetdiku.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3isnywlio.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rxdcderm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gadwnbfv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vscaqvss.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ulglratg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gqijvjfv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dqbtyloh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3lthnoqiy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3chgtsukb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bqopfdfc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jcwrjqmh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lgpvicuw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nqhsujii.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hicmzkzc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3adihpgqh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xwctexkk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pjnpnuas.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3dgayoqcx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wbaaiess.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pkzvgxzx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3byrqvbrd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jekgfdwy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ailegrui.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vwelannt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vsvhkafr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3crgdcmib.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3uavqqfal.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cbgwyqta.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcfpemgi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kdbzqfyz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3apzyaxwx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3cpefagci.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3iggwzlhe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3lopbnuuc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbgjbmfc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3afbovzeu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3jypoukju.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vrvzdlvn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bikqaiek.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ccvidqeb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nnhxlraw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vzbwlkyv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3axisanfw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nmwypykd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zujdibgr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ypdiynnn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzcqeqep.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiwgsdmp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsytccse.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrodoviy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wimvhehe.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gjwaknve.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ncmjnsem.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3juxcibhr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ygbcltby.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3odrkjupy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vbvwuzty.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ljmbngpa.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kxuubhwp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xpvhzolr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kujezcij.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3svicmmsj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3oyrwmsjh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jdpumyoc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3swmvxnge.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tuqzdovq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3avalueod.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3relupiru.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3efbmliev.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3azujqbad.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3uktjaxre.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fptvjcqx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dkmwdygk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3djwzzmug.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mnqwuall.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3cawjyyxn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdyaawla.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3fzrnzzqz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3tnlcvrro.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3oxxsxnjw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eenpgqbl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lrhtvsbk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yogovabf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ygtapzzi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dmhookfv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vfltbmhs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cnwsjsvd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pmofxgvh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bcjqiesj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3giscqlir.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ivfauieh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ynwctfww.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3znghhhxt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3evwgxvdg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3lgloqisw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ewwbtfyv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vznibsbi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vtxitvms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsmfdivy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gdmwlrib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egpjwoil.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vqbdoimg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bhbyysxh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3suqehsmd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3exzlwxbp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3czxqkmel.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3slgycptx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bsjnbcir.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gwzmjjjq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnmwttrw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ginqllpm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3puaapeok.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ckjartnl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktckixcq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cixbqrkl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zasrywrm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3lyzeeqku.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ekidvgys.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3adqnmpkb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tfadoiog.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3dvevaozp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lyideloq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xtuzxykg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jvxahsrt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3apfquvbt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xsiqjidr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pcdwzlrm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wpopbrhb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3dqtxehoo.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rqjzoqmx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hkjnwutm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3aompvfyh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3aqqjalil.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hhmcynff.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wshyyqoh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3hkpwjuex.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3afkuccrs.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3djkghvdi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3earysrhf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3miauagru.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bwaaoxzc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmnwmtvo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3auwmhmrx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jncykhes.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3vgeurimu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vizhnbtk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3lqgqkobh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3mzjvnwos.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3trjrnvbx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vhcninsf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fjxsfsvd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xfjwpwys.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3diytraqx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3hinmkjig.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xbxpbhld.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3rymsdcxh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3cyjswysj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nvccxjoh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3epygcgrc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ynovcdkk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zmmhxhkk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3yaaqsdod.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3dbyqkvgf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xpdpqqex.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lhjpihzt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ptblmiln.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dcxxzrem.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3swbaqjmh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xtbwoqlk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3dithysdw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3oisgstkv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3drsahtty.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3esjiqldg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xenagzne.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3hmuibqiy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gtjlxise.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3txwfmucd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ylobotsf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3cnwyzvhw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dhqxfnpb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3geezirwi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3dubzmdxt.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3utewgkuh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3uujlwquw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3dbprsiro.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wsswezle.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rkukbcqf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3opbbotnj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3qdzyzrma.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ertlkpmx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qvuoyhys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qctiduhj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3zriwuxdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxqqvkby.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3jrqykcxk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3axxygjxy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dxcedryu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjvhxfxf.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3frwxujpc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3bmnzmcid.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swfqbdmm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3czisgfyh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bhqakxsq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fkyzhuzj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3tkvxkmcy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3bwazyoon.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3tekjurfm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ssopzwge.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qnhcydlt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3abhtvxke.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hnzaikzh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ssyqomkl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3atahcnvr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzhfrzty.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3odxfauqw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3jplvcepk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ekdbawfm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3vxnrhbcl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3eknckgwd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tpxssehl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3wnwxavzn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3fmjqeskx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3znjunjrp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3symsdlzs.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3eypzanwr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3imemzdkj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bkevxxmb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3skwydzjj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yjejenck.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wenadjlo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ygdpudic.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3mgywbhfg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lonjospa.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ozopxoty.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pxnlkcfu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3pioqtuti.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjqmndtm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hcvipdzo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3pxjuvbjx.html


<!-- 参考信息 -->