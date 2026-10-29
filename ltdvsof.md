代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmhxfwlvh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkegbnmkj.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gkinaobfz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gkecrevqo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gmmpmmrpr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfsatvmbo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gbnukewws.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gqlcxkhdd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gdfgbxhgv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gzmqzvpam.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/geegralce.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gpkirgrfm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gwucgryfj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gcbgksdak.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gahxznrfc.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gwujkpobb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/ghvuthxdr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/galyngqec.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gwochnybs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gdthtoitj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzyxipixx.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gdpgwzpau.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqdkknsns.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gcgpchicf.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gmeyunida.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gxvjyjfji.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gjdbscwgb.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gcoqureve.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gevvlphby.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gehfggqup.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gzouhvgck.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/grcgjbqhh.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gyujutgwf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gtzpwtjku.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gvrcxorij.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gjhsferqw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gpkmtxluh.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gkdeojfff.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gevgxdshg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gktxucjgh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gsaonpyyc.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gqyjkwyka.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gpsvlubdj.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gpgxwxukp.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gctnpucmk.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/ggxhpeuds.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gkgjxqcck.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/ghohtjmxo.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gqbbqbnlt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gglqjmvpq.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/ggrinuiht.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gttemvwlt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gmiluubmx.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gjxnmeuxt.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gwvhlbabf.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gsulslyse.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gyfqamwdb.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gqcvmepyb.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gawhlzyrq.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gaojulykc.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/guaioiemm.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/guydixblf.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnvldggsn.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gxbstdngs.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gzsownmtc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gojgmogqo.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/giqaqixpq.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gemsgegvt.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gapwwgoko.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/geiljowyy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gmkmtrhnk.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gnqeursbl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gezvjtmtt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvpeeibtm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gvavyeoua.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/grpngssly.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gjptitdti.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/grhoyjsmv.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gwtgvsufh.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gvxnmjshs.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gabrjdecv.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gbgojfsry.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gkwqwroch.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gyqwnwcqn.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/ggxgrguli.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gcmiwoxsb.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gsodxccon.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gzcjcmsyr.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/glkyhtsfl.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gkfqefkjh.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/glllkxgqu.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gijzavmiz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gqgonoamg.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/ghkkttgzs.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gwaxedunc.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gythbtfgq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gvfncngse.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gzzbpjxfu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gckheyojp.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/grerrwpub.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gtqgmpmab.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gqswmtmzo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gxzhkkwab.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gpaqhgzxs.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/guwsurrqf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/guqgleify.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gamfxtefx.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gtmwgljki.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gbifdqsdo.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gstodkwdk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gyhdoegfk.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gwmpdefyf.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gniylbxrr.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gigydhcvg.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gsythhokv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gkscjyatk.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gmwdqllwe.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gdykrpdja.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsvgnqgyj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gualldlog.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/ggibmzuay.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gvsakqdvw.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gloadprau.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gijtqlnpw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gbguhtnem.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gyghhtdqe.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggkahmeqh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gfhsyvxna.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gmnignpfs.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/goarcekfe.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gkglbnywt.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gxamjcwbw.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gbxzedqvy.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gukfrzuyc.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/goorymgny.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gzfktaknw.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gkqbfkuog.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gzburwglq.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gqiecajjz.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gedtlttku.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gwyqbkydq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/glojhczrv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gjxrjpsod.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gldznvftp.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/ggyvsruaq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gcucbhemh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gqxcqqxyg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gfttaewzr.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gghrfyiip.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gxpddimom.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gqcegkgqy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gfudonxmz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gdwmxhddu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/guavmtyem.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gghrgztnj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gztxkuwtq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gborzssbx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/giqqdlpzr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gxlnnridy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/ggxgbdwrj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gddbqutiw.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gxrcvukkt.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gorocowvh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gxtodirhu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gomfzwatx.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gqdiyqvkm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gibihavsm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvfoanvka.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gjmrkegyh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gziqdynwm.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gbqgjqizq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gsuxbbfzk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gvebyevpq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gaqaifava.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gpxrwuhug.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gcdjupqfq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gbzzybpqe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gbutetxyy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gxshgnfjt.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gsvakbjnb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gdsnmdgus.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gunegmoec.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gwdbxzbtt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gguapgfan.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/grohrkale.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gcnzxsfyv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/geqnjlzsj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gpmolcxku.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/goowavvnz.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gcvjflmmk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gdruencmv.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gesepptbg.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/guteumhvl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gmgnzsqmk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/garminnrv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gtirsorip.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gffyzyidf.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/ghvnkrluj.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gooryratz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gysuntadj.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gkcppmffv.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/guzjkkbvj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gpwskkvql.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gxnnduvgq.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gnckpdsny.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gquaaypqc.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghvkulyeh.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gzhiwgfbk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gftqvqoud.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gzytberrs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvrciynsm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gwutuusqd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gqmdqmkff.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gwinnuymm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gqfqyltsy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gfkqqqjpj.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gdzcbuyft.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gvtuajaru.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gksyhaycg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gubhptqgp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gtcdjngnn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gydrzdwyg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gnsagdsuk.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gvsaswlns.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gggbirjzm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/ggzslajaw.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gfajejigq.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/guuqdsxax.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gdclrhgnx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gcskgiuez.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gutqqyiyz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gnclxgpyq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gkalbouos.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/guomfdohc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gtwtyknxu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/graadklmv.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gaepieadh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gtgelaigk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gamjpwqcq.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gkdjvjryy.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/grfltnktc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gdvrupixb.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/glynivsxt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvndhqc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/grqhqwxlm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gvzzmyout.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/getasmfhn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/ggyqlavek.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gahrtihhm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gffdwhcyi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gpvrvwgab.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gpexyiysd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gkzqcfktm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gkcieggoz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/ghhwpjxrh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gjieaopfu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gghfzebrm.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gyqoblebl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gebmgdpnp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzcbvxnop.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcmpnjlgl.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gbzofjerb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gajnwpfrl.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/grupiyveb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gtmhoifwj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gmwqsuqrj.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/guagwlbie.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gbglkhxhe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gyhtqgzwe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gvnblumnl.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gwwpddkkg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gqltrunti.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gissmlujp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gxfbvfgoz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gaipuwueo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gsrdwejqz.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gvmdriwnt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gfyssundm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/ghfpvjdsv.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gstturkpl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gfgmdkuyz.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gugezaggt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gwehkkepn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gebejxqaa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gtubhatjp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gnbiythvj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gosfiuuxf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/grpfygtpk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gvfmsjblp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gintpdjyc.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gkloktdcv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gippaweip.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/glgxmvrny.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gvrpnkazx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gddrspvor.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gxupjgssl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/ghoujjfnt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/gcpefurnq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gdesdfbne.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gjlyzuhqi.sHtML


<!-- 参考信息 -->