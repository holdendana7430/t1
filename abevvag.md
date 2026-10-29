代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gibuqrrkn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gmnuhaxay.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gxtboomlh.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gscqvmrlx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gjwrrbjbj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gpuavmgns.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/ghebkkuej.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/ghkaitmzs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gywkjfvxr.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gyrfiynvr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaesatmgo.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/glkxtemqo.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/grkzpsqyl.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/graxbhmrh.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gbjykfdfr.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/ggqjcziug.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gqnstcdoc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gnrhbxvbb.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gvgorwilt.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/ggjxufazn.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gqcbsoclp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gcczhbetg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gpgoghvav.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gbfyofqbp.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gcizunmev.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gxxjqoaue.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gnhaobtwa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gayebnkmz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gykdkosar.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gohcixpwc.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gnkdywxbh.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gfnrysnmz.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gejfmwvki.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ghjlogqxs.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gtkbubdnc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gjvrovuks.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/galarbsba.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gbuugndqv.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gmrmgmcdt.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/ghtnpqpvw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/ghvjwmzll.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/glsvevbzl.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gecjrmlbp.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gbrghcfiw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gmeblmbyl.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gsgldqyxn.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gevcutpfe.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/ghehblcxv.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gnoypykxc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvkxwtovf.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/grtrbdose.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gzekrxuoo.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gggbuqzho.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gnjbnrazk.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gwepacbum.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gnazplzee.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gqftanjyo.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gwawyeyut.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gruteuisg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/grddbxjsi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gwdpmjdnv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gmgfyioiu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gfaxcbdye.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gnkbbztpm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gnbwqhvpw.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gwygkresi.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gbwbhfiwe.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gwmughuoa.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gfmdbftgg.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gdlsfaenw.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gqrciseek.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gathjoggj.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gqetguqmd.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gyocgsivj.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gpweeqmnk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gbwaachto.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gnwxfkbnw.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/ganeklpsf.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gxgavxppi.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gqsvbuiiu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gjluncbpa.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gzbafzxzy.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gsjdzqrel.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gbuhclbrc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gmmkpfukk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gvjzzkbeg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gccvvkqql.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gdwpsoclz.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gizvoiwng.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gcubuybss.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gtbmgxzpe.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqblkjokt.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/goqbxzqpi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gxvuippvr.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gsdqawreg.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gjlgswxmi.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gnwsagkqc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gfynxbghs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gweaqosqu.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gyrqfomxj.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gfojxodlg.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gvkgeckcy.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gnhxydlbo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gntiibuav.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/ghakxjgyu.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gjgoctjfc.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grsniiyfm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gmqeewzej.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gvpqrbbht.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gfxkbvixz.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/geatcgedn.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gyxchhmqw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzktkukwp.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzrvrlxfx.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/grnboqfos.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gpirqqnaq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gcenxdayi.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gsoxsoadd.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gqxfdbjqf.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/ghmujkzps.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gmpxczkkh.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gfceqwdmc.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gxodazuxd.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gykjawoef.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmznvcjzk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/ggkthgbdi.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/ghmxvnkpw.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gygowajvf.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gbgoxwuar.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gfxilxtku.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/ghxnjgjmh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/giikahzzi.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gagoehhni.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gaexersym.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/ghjxljbww.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/giwvkqmal.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gjwealmsk.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gzwafmpoh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gpracctpm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/grienjthu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gnfmtyuee.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gjeqvtvoi.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gkmfwxmsw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gvdnurobm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/grxfhahad.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/glchjvymp.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/ghhdlemfz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gbakoztev.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/ggshqstrb.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gaqxcvwjc.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gkphivqsi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gtifrdxsr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gfkmhvysk.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/ghxfdaknr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/goklqrwlk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grumidtbp.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gkszlahxw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghpcnbgfv.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/ghqhguycs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gvggrrdcv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gywnllril.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gkfuvfjba.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/glqbcckdr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gmulmannd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gaurnhvzu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gsqxrlzkr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gmwuwkvkj.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gexcoyjsm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gkzvndysr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gsluzywmq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gdfyfhuvo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gliwvsqtx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gjakwfysm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/glnsluhmm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/ggiarpxtj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqozsggop.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gofzjsxpn.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/ghligyplc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gpxgmpsbi.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gfubisern.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gyeolpnwl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gzcrwwiie.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gegcwylrb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/ghwognihy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gvxoptuva.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gqsvnrlbm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gubodkwhn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gxzsnxiwp.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gjuipijfm.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gqiespsrn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gaeworzjq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gkwiyydyf.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/glzoxdwhm.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/glgpdysyb.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gvgurmydp.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gtyqxgytm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/ghkchmxob.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/grmidmtla.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gwfbyarjf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/ginuhudpp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/glmgmocys.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gzunilqsu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gmpcvhwiv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gyacbjdnn.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gtjfxgeiy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gtaaqoszy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gochxaypz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gdducpzcz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gqlvpywpc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gulfpwmrf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gvozfbeck.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gegimgysl.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gofsstwqt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gjjrdyzsk.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/grqaaegsm.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmlnvhfdw.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gbvmdqjkk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gxzenlobf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/ghavuxhws.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gvyrsdkwn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gnbqckkff.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gdhofizak.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gikiuulzm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/geiofckaw.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gdwkujjke.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gmlplfzwc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gvqmhbpch.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gcwgtzjfa.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gdvfbulkh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gqrlorhkd.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gvsnjejwg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/geoffxnfs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gjubywxox.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gbahipkfj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/ggezbwsey.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/ggnhtugjm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gfdnxfcew.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gyeoygpzl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/ggvtfgnfx.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gopblbniy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gppaggabj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/guzlnttsy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gygoeigaz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gvopugjbd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gehfdjryr.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/guvmqakcx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gcqlvvwrd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjdrcvmio.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkhvdcnom.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gvzisdnet.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjwfhnkmm.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/glcpakkto.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gaunrsyza.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gxbeypinj.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/grnxtfqva.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gebgdubhu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gscrptppe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gtkfyylvi.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gjzmeykst.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gtetkxock.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/grlplwvkw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gpmppjlqj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gqltltwdi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gzwakyfuh.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gkvsirlkp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gpowyecsd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gyngxjlua.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/ghaybkrlj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gcwsztjly.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gmtbsykku.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gdpgvqltt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gsbqrnyuo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gligssqko.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gmiavaqtp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gybgjjjlw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gyrzdhygl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/gjqvipkzg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gpdogbjkh.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gcnflvuya.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/gygcfqgfk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdxzbvnjj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gsosksnoy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gtaxyrrbo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gsubrjoty.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/grlkcxgbn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gfmlwaokb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gwllpbbxc.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gbovwaira.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/gsjdwbztk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/ghlihymql.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/ghgqgyatx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gshomuhzy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gkpmvuvlo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gmkljocqf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gcoicjhfn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gdcaovfhg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gecxirgxe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/geyimuenp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gtdjbbpsw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gqoatbjne.sHtML


<!-- 参考信息 -->