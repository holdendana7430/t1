代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hrkrswkp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2omsphaiv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fdbdjnjg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hlcdaizn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kazzutwz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2aygwvccs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdbnbyju.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2udrpvmoc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wfovzvte.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xwcqqpnc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfgxaowq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2yeytsmzr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tmjhgurc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nojebiqi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2osejsygd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jtygcpdw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ugfffeep.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ocfnailj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wdnnwott.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyiuxlhq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvjhzyyc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rhaahrxu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2cpwvtuka.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2trjtqxzu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wvnszbue.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2dekfjkni.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2iqszvnxw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zprkpcut.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yjilhhbt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ifijnjzv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mkvxnewy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hlgoekwl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pwekluxz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2eyvvfswd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vefyvhpf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fxqgwukx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bptwmjwn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tghegawi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otkocvwy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhmdjccb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2niqpmacw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vvslthqc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vpvuswky.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2mbdphtai.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2lcipetvk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lndvfdcz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtjijain.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2avdnlvjz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jjdgvgsi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2vrdfoqit.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2dqawjpka.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqlnldif.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fchqyfne.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lwdmbxwl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2acidlbmn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2khprofcu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iencyact.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zodwlchb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pnzeikqm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dboflfqy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2cawiqvaz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2cjbsikwa.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qclsyoql.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jazgwtbo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rcmetnvn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rlmgkals.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dqancdqy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cygehedf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2brddmbek.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mkinsyrw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ufczswrk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ftsfityk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eoulydhk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rrtsfoul.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ptvledeo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2shibxmgi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hxigefok.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dceyeihu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2krycrpey.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zcflgnpe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2heunfgcf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqvifjnf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2agruezyb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2aewfxvfb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuhmuqlj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ifaeazjj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mzulpwxk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yvrktcgm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xhborsir.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ziezovjr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ilyzbxxg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2frfgkhul.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iesufayy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bmxqqakm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2niadmlpg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2beyzjsvx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cqqlmzdm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2mzuuyzzt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2aaljaegl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvlotjev.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohkywuid.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qteoiwvf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvitinqs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uzagbugl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rlwjidkl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2leycjacd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xzxxedhr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hllewgmj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2viikefdz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2haiufcuk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2etfnpyxn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ucscherz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fjtmguwu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pzpobnir.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gbkzgfnn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2pvdpzahp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2qtvjlnqr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wugwvdfd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zvgligtf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qajobcwu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wiegvksq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xjwddkps.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2syekupur.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vmhyhbxs.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mxohiwlo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kiklptea.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2noniwkdx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zvunmmui.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hbuzgeix.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wdosxaaj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vokgigai.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2giepwsog.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2tasxypuc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bestmsrm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2blbbwztg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ixloacbr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wlvdrmfp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ymwlpfet.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2gbbazdze.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hdodqliv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2djkcgmuw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gacbpbxx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xbhicutf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gaqosiky.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2iupppdbm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bmejsrsn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jtcrpghf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2iyegvvrd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2lfixcngr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jsjmfewh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2grjqtafg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehljydhv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fagodxnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2biafrxgs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tvydcvlz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zobvnkhy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wfdprflz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2azufxzhe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2youjdzth.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ygqiqpxc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2flemtoyw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wvawzagr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2pojsdyos.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ddhharow.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2enfuwndp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qflvqspk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohiimudd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yxilnjjb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlipqhka.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gsvnskqp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2mrapiysk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2byiksnay.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gyykmjwr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2gxxgaeix.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2luitbwvv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ypzpysca.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2phzyxhns.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gxrwymwo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2kwukwwiw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fbflqkxk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ihezwwsu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hhpeybdg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bknzpiby.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2coqbraub.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvqvlemj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycburxnk.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2iflnshto.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2mumamsan.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ypvcwowo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2czimjqgs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2rcxnkuxy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2gddacokw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2daxgnirg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvrtgtrg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbnxuxai.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2fnbcglmi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2yjcnbcim.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2lwhiphwn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2juvqdowi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ijfyoefd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2nxqnaxom.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ucqrgwhp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vqafkwwr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2urfcqrth.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2jlzrjoic.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2rojuqbxs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2szorfsqk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jqoywemk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xenbshcj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gyobtjpo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mniibzxq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sjdarfvb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hoqhfwbp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jyfzmzyn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2mnctxfsk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ijwoemqz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2phpipahd.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2xjpvteeh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2bpkxuayz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2bujvyjzv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lwcbpsth.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2lelewcuv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2xnanbffw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2eqwqfbln.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2lfetacpc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2wfsnjrqg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2vrdvnqfy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2keewzytt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wlymbxnh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2kcdwbxgj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bfbteykv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2eilkhvpg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kwkvlqcv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2pdshltgy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2oeedlvib.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dnfcqhxg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2uomezaka.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2isffxdep.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2yqlsfmhk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zdhshbms.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2rutakcru.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2aqbxegbj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2vhjjyime.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2toeafihs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onddhrcg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yssryebc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfcbbqdm.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sepdtmie.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2afefaksg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tyzedaxs.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rhyhvqqj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gwdtvgxx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2fwpdguss.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2mzrslpcb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2qwoaagyy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kgmuhzfg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iakoinzb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqgwuugq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2widqszey.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2dhhkchnj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2emgmieea.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jgsayawf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2curczwjd.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qtcieviu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ipmbcjrr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2bdosbcnd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2brvdpnaa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2tppaqotz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xlzzvkkl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lpsesddu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qiqqsltz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2dpsnupvi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aapudzfa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2bpaqnvdz.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ejjygqbx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2wldwsscr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2snigrmtf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kzgswfzp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2iedznxwi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uaawmyod.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ccuvnouu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2upikrvya.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nhtrnlxd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zwyqkkou.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2soeqsens.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2agnhwqqn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2viyxtpml.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vgcfrkom.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2rqcaphth.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2hrlvfmoy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lsuxlxlk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2rxrcpdpc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2fwuejmga.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2esvhjtqa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2xiqgzcug.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ihmdeqxg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2keagtkqv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2tdhlaeqm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2daqnpwwp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2hdfkmqhk.html


<!-- 参考信息 -->