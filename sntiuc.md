代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3diczltat.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3fkyasglc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfgwzkms.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ensaadof.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljjkrglv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvrcxzbw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3nnsnilrx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3akmvumic.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxbwefwp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fbzosohl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mofrncdf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzvrfeza.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wlintlme.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vljyojab.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrshisqk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xlnlfwzq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3oeemmfax.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jripyqty.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3drwzifks.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bqkwtwsn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qjzzgkpn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vlpxgumc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jjlsavbx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nckyoupx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xqsyfmgm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3orbfzohe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3rezigynn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3pfqpfebw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmyozhip.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mvtrzsxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxienquw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nzjnqmgv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3edhdoqjt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3rgsaanct.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ynqoaapw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzxiizol.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fgielpvd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tcucljgj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tjccuuve.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yygkdhbn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfyoufnt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3pykkzflb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjpzkgzg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuwvdfjt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qrazcsrg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3htldudnn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ffkjqhmm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3diecgoqr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvbilyll.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3gxnlglgk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mpaqdcsy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qdbfeoec.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fxsbehkm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rfngnruv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wsuxbszi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rldkdodj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rknzwyqa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dhbglttp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3imycicwe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ildmmwqh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmefzpza.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zexbwvkf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpyihegc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hotztmfp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ladizsgc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ptirsxqb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kdcvlibx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hovtceiu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fzagwvmi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3geuudxcp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ieonxhwx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ajiqlpms.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sadpyvpz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ggtjgwyh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3optrhniw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaukcaox.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xppxpkzy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3obformtf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ozdnpkag.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rtfxrhhh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nltlvukx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3flitvlqo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3sxxcivdf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3izecybqy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3gheaponp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xebsjqrx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3gbwmejzo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3oxjsaoym.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wwltksgu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zfthbnef.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yzbmbgso.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3oxhwzzmc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fuddynhq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nllisiqm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3yaquwxzi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bjkbvhix.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3lktisawa.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytgxyndm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vijvwful.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ujfermip.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3uobsogto.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yysftqwg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3pmvirqdp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yhvfvfrs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vrvrlsbd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nsqiqypd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3buollyey.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3maicajii.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrzaflc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xychqgxg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ktqcwnfw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kpenzajt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ggijozlq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3viotgclv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3thgainwx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gwztmayo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mvqiehoq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ckhvkoet.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3auhoslxv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sddwgbdm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3sugjehbz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3auoeuomb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wjqytmkv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvchvwwt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxenvirj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3efqgrsej.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ossdvehd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eokygsbv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qzpiwozf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qmeotpdl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3savwdnvn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nnqfbuoa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgcwndke.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyuuhwkz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fatfqvwn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgmdicfk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zwarrdto.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ybijlrev.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ijknqqky.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ilhtzkqf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mqmpraof.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cdwfpejq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xxsubkqu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nciqysyj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tfyruwva.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ryapgrfe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3tunraqtu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3acqyhhyp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ileecqma.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3eryxganw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mmnnldkk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pcozclzo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3emqxgjcp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ahzebbbi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bkhtomub.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vnmsvykd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3hvdtyiqb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ejsqwuxs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hcclkjcv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqsbslsl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3sekhexmm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nirrfekh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3yzowlpnn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3lnuezuti.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qzwadryx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kddahxei.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xelkryfz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3cmzyajfb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zafnqfer.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fstlzsbi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jkdmuokw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vqjhaaeq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3waydsbab.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3cqbcbkni.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lqzfstfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjdqoaxg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3eqsrtndv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bheffunz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3krwynsmo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ckjviarv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3zrtnsjam.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bvkydigj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3njcyruno.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sukrlgvm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3pmtnrxmh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vekshuoa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kejfnntw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ovroerrh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zydcvqed.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwrrvjas.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qanxpzmj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcledabq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vvoonioh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3druxpwja.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3bdrqgnad.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mhozuaxr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3khjgswoj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wjwmtbrw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zxsqirln.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oyogeirz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zggppkqx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uovumydh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3vazobemu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3tlxtdwpm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ngojiwly.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zjppwfkz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gxjureti.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3svfdhhtg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3esmnjflh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3onkkxnoq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkkvbpcj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3psfputwi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rfukarin.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pvwugqfz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ptkggfyw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3lgjuyypr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3vmrysfbr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3remrvisf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkmxfkug.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fygjvvjf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3nbuniosg.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3kqypfcae.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihgefrco.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3rpasdaxa.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3tneijswk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ksssjhhg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iizoosem.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3obdshiax.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3pndwoifx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ytpfwznk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3bityesdt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3tknttnqi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hpdmlnhw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lnqzlnip.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3japuywku.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wzpyjqvo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3utihpvof.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3gejyeuwr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3cfaqpnyg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ddufxfcm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tbnysesb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3oaseiqzg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3jhxgihej.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3mkysjeyf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3adpvuzem.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3itmofryb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3zjzmxmfc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3fykraupy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3snwimhyi.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ccewxclc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3owcqkyyd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3yrlqpdhy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3gepurzhi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ujcmujiy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3popclmmz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3aotbazoj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3gtveefou.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3cfqkgeke.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3mesattgm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ibearbfk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pvvapoto.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3nsmtznkw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3shyhtuio.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gdmcndls.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3psdfgaiv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3npkbhvdx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qmzjfcvs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dohbpxbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvlsdoec.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3xuuunikk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftfeiorx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3liysxplx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zojlwado.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iliyintg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gzxshgqg.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ztdvnkei.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3fhzhxiud.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ewveznzz.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hkzujpaz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mnnpsdor.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3payfhgmi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3debtahqb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3spqcptuw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kvmnhmzl.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vupvdbrr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3pnxyrzqs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yydrlgcn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zmzfbslx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3joedomcu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3wwyhhfdy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hignacuh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3spbnnhyc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cdvbuhoy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3anfgfboo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lqerflge.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3khahoskc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xbjugqyr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3oduwsppk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dwobvtxa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3uhxjhjyg.html


<!-- 参考信息 -->