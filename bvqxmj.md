代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3guowpnit.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwrfcbjb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ogqxlciv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zmivoizx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qdcpzpdf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmoyuuis.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljpndzrs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ggbyzfho.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wymblfdl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohnbfrmw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ioixdzfs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3nnxpujhx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3diqzwtvo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3eclcsxqf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3sqxytqff.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zoyqnrpk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qmchhmdz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ftdaprkk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vygronfy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qguxwavu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhdxtgaj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hhakfebg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kykyapdq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vzuojbtw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3vqedfzpi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xrfekjiy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ruyikruk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ippdsgmp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbpttjxp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fqvpolrq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3toktlinw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fscqkgxm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3dmwuujlc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3omiwhupv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyevrtbx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqpskmik.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ooxzusjs.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjxnnpbd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lnxzqmwf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrbertdv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pruotkue.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ziejolpn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ukyyjttu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bgrmnnjq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3radmgxsw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zvrzwvuh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3byuykedl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3sxzbxrii.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ljhsnkxu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kigkntaq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ivcchstj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ppnxubgq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sjwafdva.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkmmohqo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oitnraxc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qfcywfsa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3exaydnhw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gptgmhgz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rybhotqr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gxmndbrs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3upeqvmyu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhdtyiry.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfzndagy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fygjixyb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3swonoimx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wqwqyquv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rcfehrea.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3kxximely.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3pxtetnaf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3apszdfbc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpsoyqxc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmcgqtpx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fudronhp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgjcxdnb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rvvnrsui.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gbrxgvvr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tochvtfk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3yqhsbegp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3iwblrvtm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3sqftfohl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yedhzhay.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zlfeucqf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3maxxsqcs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ntfztbud.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3alhihdcx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nzznkcct.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3aemwofyd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3pvypicyp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hoeiuyav.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdxtzfwc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqiosfrv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzuegvzo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ejmpqndc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3jvkepyqf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3okylgcoe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ubbwljge.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ezhnckff.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3pedzljxw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wohvjctx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3uzuckqry.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbkolmbw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ixbsuify.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jwtsbmui.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjrvgylz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3fonnhigu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gflffxiu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tsnhluee.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jbnejvxd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dwjccgrq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hxntltnf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3umgdugui.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nxhjmvwq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vanswqyd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vfbgikkv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bqbbtsbi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3durdbirm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cxpwrshk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pgfthpos.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkpybbed.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pszsiwuq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ybptlbau.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlvirqxn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3hooynyeb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qyltfskp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxpdzkdi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3slxulztz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3htlwfhic.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgvwnmey.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vzsjhccs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wlwcirao.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3atvbndxz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cwwoljpr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3pbspkwqc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iutdddvb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3slwavfdj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fyvwmcvc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yzwvrkea.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3bhmbexjn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3zciehbyh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zrvtueqh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3avehsjlr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fbfdgiuh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3yvticggn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3wzeyljco.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vzwuhiaq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lskbdnfo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3szeqcdcn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mfbgbaoo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3yknodoum.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oferwzzn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zfsedrmb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvqtwrta.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3draflxwn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3uxqvwkpt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3gudylemw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3iqdqouiu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3gzzsllty.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3djpzurur.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3jaktdhai.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gtbgleai.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3lqtmtbdq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bofkdebl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gzugspww.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3qmwnmibd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vcctewrz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kamtaaaw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3afifegxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbxuzdnp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3cuzuvirt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ciqubeze.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3anjobepq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ttpopjdq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhjzsdei.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3msnentbl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3trzujjjw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3mjilestk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kumbzbip.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3znfcxmcd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3fargkuzp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3nblydpof.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3chtusaam.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cexhjgsa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uvwxvsxc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3htarrrar.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdlzykld.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3qgcnrtfi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmqjqfts.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qkvarnst.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zyjrqutd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3hlqxbwjn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cpjpnoey.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jssaaxzq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lxymhjrg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pmabxzxa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3liglctvt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ygwhvchr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vuehwrfq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3bcqztkuc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xnehmpca.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3omuojprq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kswqtluz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzthmxif.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3deqzmlqm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3rusynjvd.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3walqscxg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fckktqmt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3clvpdrnm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ziicffyw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3xvzoyyhq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysmmtdcm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bfmigggr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3vxfinkof.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3sfyimovh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3lnkiwbuk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvjvomis.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3nlazjpcr.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pdvdwsxp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dsuuywif.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jfurodrq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zcrzjluj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3fdydtcfc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3fdjjamem.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wsbzfzom.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3oxqknfzm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3pagqcuup.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3uesqsnnv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oeumjifs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zcslnbrw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dkplmxmz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3txnplrnm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3mlxckjnx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3gxmhqouq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3arqjzsah.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3jxryxxbi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3iwednoqf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qlpynccc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zenlhteb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lfcsinbi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3rqcriuzz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3qicraorw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3nflpljly.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3mcvjnepu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ekssyufu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3pcgrwkzh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pltrkwxj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ldmbzrrd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3oovzpanm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3yxpzjqvs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3myesvbrx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mpscryrp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ajhsawnq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3kyvmdyuq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3hyvwzadx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ujjqqeua.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3iqboucmb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lnxtmlkh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3mroxdnua.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3bsdtgxmr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3cruiccml.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ftssfzau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxvrsuzy.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3kfhkfqqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjystvqx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3qvemdgpa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3njvkbapc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sifxseqj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pltugltb.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nalcslyg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3gqtxubys.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mufkaxwm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3rowfltgm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ktpvnxep.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3umqkirtz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bubcuzqc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3zdsuawdp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3xvzinyxb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3sdrchodz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3tiiumlad.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xglwstjm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tieqydgs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3opikmsfv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3exvlnfyt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wonzalsz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3cledjsqo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3nqpxeijf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sngkhnsf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hseztshr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3vuizcbbt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bpcwyqab.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3vtspwnff.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3cnboguyd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3auwjqofa.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3znsakkcj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3qabyykqq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kieoipyi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ulzmicnx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ekepeqlq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3krjrojol.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3acwehggj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zympiaic.html


<!-- 参考信息 -->