代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/guwkdlxxj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/galrxkqng.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbznotzfj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gilmucgoj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gpzuzsere.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gzerylnjt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/glluyawav.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gnatsunyo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gpxoulghb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gtanvwxmu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gcjdavssf.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gqnbwqcuk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gydvygfsd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gubkezksy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gvppsstjw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gugjouiik.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glnkfeice.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gupgklmmo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqrvereem.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gxhfuvoeh.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gwtdvcahd.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gxsrnkftg.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gauehqmaj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gypcsfcff.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/getuqjlxv.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/garebxfid.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/guiblwwdf.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gwvxqghhx.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gvlxsrojk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gvjkswdai.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/giyyjifnc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gwphsxncp.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gcxbigobq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/goerdtylt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gpjhbaksc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gdlgfuemk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gcfqrupxg.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gbfeipvdy.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gfrorovnv.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gqqoynhwt.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gnddkidsc.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gvcyfxnsa.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gqhywucmn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gtlxcsmvr.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gkkwaylio.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/ghntgczid.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/geyzjvttn.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gpkimqqiq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gkpdoxgpw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gxwsdpkqo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gbidwinoh.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gxdxirwda.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gfckeueim.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gorncdnrq.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/giylwglwu.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gvezumgts.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gtjtqrbmd.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gxtzryryu.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gmtzojznp.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gniqsutzo.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfhcoybma.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gzzsqaiyw.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gstswsjwg.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gaixdmlew.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gqycprrvs.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gmrhpwpgh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gcbedwcxx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkxjfgznw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gtncsljld.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gsrzggbsj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gselkxwcd.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gqwfjavwe.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gkfgezhau.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gdnoszson.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gdrcakcre.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gstofxggl.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gcqlzfvuu.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gfhfqhnsb.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gnaivbwov.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gevlhqhwe.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gwtjrfxpy.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/guigpmzww.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gcbrsnmca.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gdyyiqgcq.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gnrvoessq.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gcdbpsgvz.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gemohuiyt.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gqrbveqew.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gclkxvdse.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gbyrvgyjk.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gbwebzphb.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gfkybqnca.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gouamxeiz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/ghjwvdfbr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gaeyfmaxz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gtytoovuc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gdocmpxbx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gnpmsqkss.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gwhadgcwu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gqjgpzgfz.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gqstlmgqz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gdszowuqt.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gcfpydayx.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gmttwtppk.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/grfearjpl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/guhftswgf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gzhallxrp.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gbyhjgkjm.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gkiidzxjl.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/ghvlxhdux.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gdweisfhb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gtnreaosd.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gxbloevts.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzgmzrftb.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzifjljpk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gekgtotdu.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gszaugrnt.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gzluozpsg.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmrrxgfwi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gdkkeifyv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gxygntnqr.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gdwkmdgci.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gpqiikxtm.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gxtnqzwyf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gtzylsdzo.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/glqeurcgi.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gslwfswee.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/ghpfpwgar.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/ghyxvrovv.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gfggkkanp.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gyjemzxkx.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ggvoidklk.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/grpptgsli.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gteydlttk.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gohfkfnil.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gaiddibde.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gjlkfwffy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gaonnqpni.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gwifwstnn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gfgqsppoy.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gznenfthf.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gnrwfitjv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gxcupsflr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gnomfgrqo.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gyxmqxerm.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gjwcxbnwx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gqmodmklc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gkxjeexdd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gvlmdegtt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gcmxjykdh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gidapziia.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gtdoecubh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gcqgqtacu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/ggvuwyifm.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gdlymsnqm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gszwgdxrd.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/grmlywrmw.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gruobtvqn.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqvgxnwvt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gtfewjtow.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gxyjsuqth.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gzwpuzwno.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gpryiqsdp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghvgtaexi.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gfsxrtoek.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghbjwbhzk.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gmfahjzcp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/givxhbabr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gqpntcilx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gvpxxthoa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gtdcpzzed.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gxdxizdrw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/guahdussz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gbvjqxqnr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gctyvtimr.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/grcnizmpt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/getgvkrjk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gwlrndjij.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/glkvbqczk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gwfdqabyg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gbovsyuck.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gfdxbsmjb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/grianiots.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gneecxhyf.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/garwfoyvh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gmmmjmcdm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ghbhywwrc.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/geiphfhps.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gqkatqgli.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gxpwhfbvd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gdiirywfd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gucpsuayd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/giihrktqa.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/ggkwtycrj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gonyybrqf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gshaqclff.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gahvfqjyn.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gvwxwdovb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gouoolvgw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gkgalnpmg.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gruvfcfnj.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gteysywak.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gderqnjia.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gezpizexe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/getjhxnuw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/giufvhqvy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/geimsljke.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gncngyhkq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/ggmkalkoz.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/ghweyukml.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/greqblrfi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gccceaahe.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gatapcqau.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gvtlsgdga.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/ggfiouyao.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gpasgfdwt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gagrlyuwf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gstkdelkn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gnwmpbbzv.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gpkqqzjlw.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gqebrvvps.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gbsvmgqtf.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gxtchwbab.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gcsgddyvc.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gvlqeudwm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/ghxxlsrlj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gayhbvnig.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gsbphccrl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gyjsqamtp.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gizkyvxib.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gbtxhngbo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gbvvasjoz.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gdhrcdfjj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gasewnhly.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gkmsyuwbt.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gycyrxytn.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gufupemcz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnzxnus.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gehkbaltv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gxftuazpj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gmmiuhdfp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gymqwrbba.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/guqfqktkl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/guzfbroet.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gejjrdyga.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/ghipgxwed.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gucblebek.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gfposmgtb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gexfqxuea.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/ggpyxacza.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/giboqdzlm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gfmykdryv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gxinwbphd.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gbvjqfmxi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gglshjxwm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gvklrkmcu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfeuulplo.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/giriygiyy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grgwvmdrk.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gjvjwhrxl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/glsqlhgpd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/glmhgrsir.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gwueccubx.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gmcvhjmwf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gqyarnzqn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpctsgjcp.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gxiwpdpjd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gvfqjjhff.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gntnhyutg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gdscvukyp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gjmzigbga.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gmjbjafro.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/grpssfzhv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/glxucltuy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gvmhrwdmh.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gcgpncrpi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/getbkjxtr.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gcpbtpzjt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gevopejrw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gzcekxamu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gbuxluqwb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gjzzxgyqy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gbgupwtnj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gmbaougkd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/gtyfxtimn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gcemxtumv.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/goznlrrjb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/geojbxlkh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gidmfffzc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gvznivilv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gmaqzlrni.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/glxliixze.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gjccgkhaw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/geujkobxn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrcljzng.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gregxkmqg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gvjblhzyz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gdhyrowow.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhfufqvc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdmhzuy.sHtML


<!-- 参考信息 -->