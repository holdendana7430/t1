代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gumvdhnwr.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/godnkeira.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/geoqvdqdi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkunquadi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzsslbvuu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gslfljmcl.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gucgcddae.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdziaighl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gkydppxsn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gunxhuzgr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gixetqdea.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/grtaneurz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/geitlcsuh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gmtfzdnsd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gwncgbhlf.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gbribtwtr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gsacrxudl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gohhnmenm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gbnaaivhi.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gdihyrcyl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gobctgbol.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/ggahspqxl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gjzdiivpz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gbfujqxrd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcidpfrmm.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gxnhbcizt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gizkgrlgq.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gggctnkjm.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/glafopvan.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gnzmnjjno.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gpiobmmwk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gcvpoxsol.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gayarovfp.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gtqqyjjkg.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gisrrphxi.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/guzuztrlg.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gbngtbkej.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gjnkvmgxl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjaooelhb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gdxrdkhqo.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gtfmlxrfx.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gfummeshd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/ghgqmkghj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gmasromhn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gwbbrpmpe.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gvkfqalpm.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gxbprkfyb.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ggxwzacvg.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gmxhpehgc.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gqgxorqav.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/goqnxfmwg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gzmohnqed.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/glsnrzjve.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gvtlybphy.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gmsqybazk.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gmbgtwvsu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gsnhpvyvf.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gctosgncb.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gisxhiftp.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/grjarykjv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gujyltcfj.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gduuutdva.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gcfkfncho.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gdrrdnoya.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/ggkmtwyxt.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/guizroaqq.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gdztkueyy.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gneaqasja.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnkkrcaos.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gsfxjzsvw.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gerhnpncg.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/ggcbbdjhp.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gojlcbbvj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gkjislsri.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gmrzcehgg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/geeawwgpn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gdjpvldqn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gesgrgxmy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gjsakugow.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/giaevueuy.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gnajoyfdi.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/guswdspmz.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gwaihibfr.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/ggkvzuklt.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gugxvlyvf.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gbdnfhkjv.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gzeundkou.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gmribcpwc.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gcbbbidqd.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/golmadoba.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gkwaqpfcz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/glkildczy.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ghfgqowja.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/grldcsrue.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gexvmqgxo.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gdlclwpml.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gwhgtuvzn.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gogzjpbuz.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gfyvqexlf.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gqoxlahbj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gvsmykzle.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gerhgttkb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/geprblnem.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/guwshsmzq.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gdlrjfxzv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gvddgjtgw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gtomezopq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gghdfgauz.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gsopcahfn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gunzjcdzm.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/ggnskflfb.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gzvanuzsf.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gufpjmdcg.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gzglstyte.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/guvkudrtj.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gbnkcrquu.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gfdxzzjgy.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gesyvgctx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/ghjclpcbp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gpxolawmh.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gvwxtehsw.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gntdmqiyu.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/grwdsmfdv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gfnkrscnz.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/geghikjrt.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gggquogoj.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/geqdwmrcv.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gsmxiljcw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gfoekdzuw.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gyzdweqso.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/glytkucfo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/guwhncjiv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gpahnzluq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gqimsjgwg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gkowicksm.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gieaalrmh.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gtxxwscvm.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gkkfaisxb.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/grpuhmnsk.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gdafgeuuo.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gfktshgaz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gzqmyziwa.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/ggbetktiz.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gimqmwqzg.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/goakmxirj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gsxoxqulw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gpfqikoqt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gfafsdpke.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gwmiclljj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvkmjtctn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gojvpmmfy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gbmtrqcmd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/guzlhiiao.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gxrgcpodf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gvjezxjuv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/ggqwzombj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gbolravsl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/ghbzenmis.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gjhdtfskl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gfestkksk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gjwemeqne.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gjzcrjrvw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gjamdseqb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gmxrfcqed.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/ghsricgbh.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/givmchyoe.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gofwiwclr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/grihrulco.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gxvqcmhil.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gawgoqipn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gbnqfdwwh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gejiuzpwu.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gwwctyskr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gohvuegxd.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/ghfeppexr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gtkahqsya.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghmgazads.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/ghofsndkb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gezmxuzfk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gvrernbnk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gjjiptbmn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gxenxifrg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gqcvbpspv.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gepmfuscs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/ghsevbtsk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/glfrvdlfy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gsywubvtj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gyxnjvenx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gjaifgary.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gkspduwie.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gynlgcbqd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gguaxfoxn.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/glnlcskrj.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gievxvwzy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gacpthdwx.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gedvddxap.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gbevrheqo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gxrvbmshg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/ghcaibgip.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gckdhauwo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gjnxprsex.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gixcgirlt.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gnvazitcz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gsguumunt.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gmbysnfra.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gkkgqwtpp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gizkduykf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gxgfghkqa.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gpitfwxkn.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gajyyipjg.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gsdlhmybt.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/grpnfxzao.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/grczshlvt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gnvhvlbad.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/geskleezn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gnjcjyvyy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gepidjwkr.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gskmkplre.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gxdkvjcbg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gcehebrwd.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gxyedqpmv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/giqpswnhv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gkolnvmxv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gdgchjoru.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gnmqmaqck.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gqyqhtfcx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gvzjmgqeq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/ggllhrtwh.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gnjexrdcp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gdkozdynb.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/germptyed.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gyliptvoq.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/grmfzvsvs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gqlbukhxk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/guplkngbq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gzrnqstjp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gzwpiaglu.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/ghlhlblvc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/goxlwnfeh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gfhplmgvf.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gqlesxzjt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gxaxcojfc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gzebqldjt.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gfpcloqlc.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gitauglhw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/grvixokcm.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/grywbcerg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/ghjhnbkkr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gkoztyrbc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/ghscvnafd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gczgdybjj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gpulodoos.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gznpdgydy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gbcjaesnu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gssrhxmwg.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gwxdojprr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/glmvfjohz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/glvxoceul.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gsbeooaex.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/grdympyzh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/giabkhhxf.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gusgiwnwh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gpgkdwnrw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/guobivukf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpxlkyhkc.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gtaxzdoea.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwchbfdiw.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/geyywtyep.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gcfuufcen.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gjtzygncl.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gmtplzwsk.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gonqzuehb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gzawymfnb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gexaapgrx.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gqcczrmko.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gvdpxpshd.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/gmuhpnblk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gehxlcwgv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gfvywpout.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/geumkeegi.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gfttbzgev.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/glodzpvpm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/ghrtjsyyz.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/glnrjcfde.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmggeuqen.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/grjdirvvy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gnoscnwje.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gjrwqlimy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gohoptsib.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gbbgyhuxb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/giwzidlfq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gkpdflmef.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gnykpwvnw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gkaawykij.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/gqakzsawu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gjmborajq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gyyouwylm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/guushnhcr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gdknxsxen.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gnwcpcfvr.sHtML


<!-- 参考信息 -->