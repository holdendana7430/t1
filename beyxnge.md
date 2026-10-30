代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/ggrckpjxq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gnhszwqgl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gimkmgzib.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gkshljmzk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/grqoobdyj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjkalxhlz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gvhmmivxk.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/geulvxuol.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gipixzreh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gqhqmskod.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gkgqogzmm.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/glmdquzvp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gpdznihav.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gkaihwavk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gxfdecbvm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/goiqaxvez.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwybgpuya.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gkagmvbfu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnydptylz.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gjhkicmer.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gfyahrtpu.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gysetvpfp.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gaydeobgv.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gvqdqctfv.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gnxapfsbe.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gtxmwdtln.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/goagujowg.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gihrajncw.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gzheioswi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/ghqsameuh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/garchtnrg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gjmoyrtms.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gbpursyky.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdpdsmhzz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gnwwdorcl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gxjsoqyge.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/ghdprvnwy.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gscpdvrhp.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gsjdpfzwp.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gskkkxzym.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gerivcfsa.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gugtsymwi.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gmqfxbfxr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gohzjfsje.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/goscdvtcw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gqzydwglf.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gjttskzha.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gkyiefddb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/grqdtvzyo.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gkxigmdnc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqbfgxdiy.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggzrmcuds.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gkioessqz.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gvglqljgl.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gvagfyzau.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gdkutzxmg.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gytxatbnn.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grxwrpcjz.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gujglpgrb.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gwbjcxqzg.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gqhesvbfm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gurdtmwlu.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gpuzclyfn.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gaubxnzkq.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/glrgrvhpn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gnfxeqaos.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gynytjuff.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbubeycud.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gnulrqidw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gfrgloxtg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gmkaptrcx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gyamqauww.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gmsorpqcs.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gqwzdxadr.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/grcvbstnn.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gjpypxkls.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gpvnqqmgk.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gbbkdasqb.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gcwnlbirv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gfsbeevmd.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gnwezwxqp.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gjwhjkndm.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gpecbzlrx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gfrtsegxm.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gvwgwykfk.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gkzxcpkbu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gxdocijso.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gadqrendg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/guyxoxhhm.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/goqvcuhvg.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gniuflygs.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/grnrhcinb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/ggijydthe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gncoyhxdz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gdjrzvdas.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/geljkstjh.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqpuqeplp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gyhmvlgmk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gdwmbpjzo.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gbuvjpnrv.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gdqdylqwj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/ginxlwndq.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gacywnjga.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gwrakrwbj.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gchtxmvny.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gsyfypwja.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gxpclwpoy.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ggccsasfc.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gfraytegd.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/ggewsdqzy.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gyvlgifay.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gzbcjtgtk.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/glvydqebj.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gkqvtgvms.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkisosrvf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gixmxcmlj.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gokjcnhda.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gplaounxz.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxnrkzlsf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/golprewmu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gllynatqj.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gjsitvkdd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjcoywivs.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmuazbhzq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gsrqdhmsj.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gbddzevdo.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/glqqlpbdm.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gqtdiiyjl.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/giumaoimg.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gznyxvuus.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/grruvwcoe.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gjdpsgmlp.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gcnjkxtby.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gkdbfgire.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gyjjyoejo.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gphcoeazf.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gmplirdjm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gqdukdxcs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gjrcysexa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gyhxpujya.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/ghdkgmbln.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsgxzkmvm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gonhkpwwl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/ghycgjerh.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gykigcryn.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/ggofeialn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/ghhnkkhzr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gcxkkvttj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/glyhutzjk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gexhkswtk.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gvfgvplrr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gcwtetjdv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gvclsogap.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/giriapoga.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/goffttrnc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gwkebmnnv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gbrymnxmz.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gpzaapfse.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gklrkyvcg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gwqoapywz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gxatifamw.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gosuedhlu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gpjfpcsiw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvjwlzaru.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gmbeedxid.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guiafhbxj.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gbvxwjdez.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/giobwdkox.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gxajpfgnb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gciqqmijm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/giguyrjlr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gspxwcfxn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gookkrxxl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/glwhpxihl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/ggkdhwyqt.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gyobiurpb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gnfaeedag.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gsujjrgvm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/glthlhevu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gcdposqqq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gavnxnpej.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gskiwhqnx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gcjlhvrby.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfeniskwo.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gpyqfxsxp.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gcqwkohcz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gdwetvjcz.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/geztufnqi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ghmadpawc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/grszpyzxn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gpulltdfy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gtcxvcvhe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/glihsfwdy.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/geycppmbd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gremonwkd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gzhguwjmn.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gwvsjlpvp.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gxrktyhph.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/ghtgblsta.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gpaahbymj.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gbjcgyqfg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gfiunhamd.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gzcyuckmx.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gaesitllr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/glcqinaax.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gueipebnp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gglftqmdm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gduxilzit.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gjnkbtbrr.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gecfsauem.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gtdzehcms.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/grjlbdmvs.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/glysknnmw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gsflurjsr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/grnfylzlh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gbomhcfkr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/glikogrgw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/ghqlfftpi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/garoxvrpw.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gaocfigmw.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gxgrlyjvt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/godwwtoqs.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gapcxvtks.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdlwtxgej.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gpvbxckwn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gjlztijgs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gzwiuuuww.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gnnljzotr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/grdphmqyu.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gyhhvdmlz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gezdfegll.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gttywnvld.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/guqobwiip.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gntuojtef.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/ggnztewgl.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gcnxynpky.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gwxzmkuxh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gzvcirjcw.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gaycaoiyn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/ggxdptuvo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gxcrdcctx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gqgooywsm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gzieylqeb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gpnedpllp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gkfnlzmgp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/glzjuuzvt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gijqblpwk.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gijucvskz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gdwqdtucn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gonjmgxed.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gdtiqsqeh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gkjglnfoh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gbgbcmqyc.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gzufidgso.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gcvheszew.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grjywjmyy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glpcucycs.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/guvagmsqx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggothycep.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/grzekohiv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gqysuirbx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gvseumfmc.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/goraznwyp.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gjzkgogux.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gvbglwtjo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaxnfnihd.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gfjrrskup.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/ggbfmveww.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gytiyathl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gfypwzuxq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gxhukgyma.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/guxrgllrh.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gaekkugtq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gvfyevtop.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gggcntzjp.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gzygacmqx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gsjbsrlri.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/ghdcrjayh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/glcnngpkb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/ggdblbqfg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/gbaxzwkem.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gdpcavddi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gvtzcbxeh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gwfmbwygm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gaobpoths.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gsoguemwu.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/gvnuqrpoh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gxiswvovg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gtzkhiidl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gubumysvx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gmjppmpng.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gpmeebwtd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/ggbbwveak.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gqwerxmlr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gngtnattw.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gptpbbhbq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gvtumufkz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/guzvfikhd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/ggqrytpwu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gonumfswp.sHtML


<!-- 参考信息 -->