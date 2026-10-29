代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gdzqhsmma.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gipczbrbc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gdcwrbram.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gsopqzndy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gozlxufhk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/glywetqeb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gvrpenstn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gtbnndljv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwytbdjlh.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gvgmxrhxq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjyhruwhe.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gxfjallwk.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/glcovwlpm.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/glnmbncnq.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gjogieuyu.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gyfoonujc.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gzqwjfaza.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gttgwfuux.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gnqtxgjuv.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gohlunlrl.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gwglbswkc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gmvyoexxm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gonvwesgq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/grygkhzss.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gheoyzqtu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghrsxnmox.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gosjocgqw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/grtxtsmlo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gbztwuwlt.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gxbxdisrx.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/glujzhnzu.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gesybhxkx.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gicnoptwo.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/glongvutt.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gzyftbhkg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gmrlzoyke.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gxeanqxes.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gnfkfegjf.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gatlhennl.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gzdtcjgge.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gahvomxqw.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gzlmdsdll.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/ghqpigdzy.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gvouxcwzg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gspviygbr.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gvadxysqg.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gmednhevq.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gvtqstwwr.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/glkpqkoce.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gqwafsigp.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gdgqgwnsj.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gygzhsztm.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/goiehcyqb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gezjmlcvo.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/ggaeiuzpi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/ghsxdcvoa.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/ggchfatlo.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gkiglknxz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gvvfhpyuc.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/grojwagxl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gavpbpxvs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gazjuiwgt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/geeitcmmb.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gjxszmnoc.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gacqokoqk.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/ggjshspgq.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gfwteaujm.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gwsgfmgqd.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gzybsftnj.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gfugkznuj.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gjsdqkqip.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/goorkpfdn.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gwwnbyzkd.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkygrkmpb.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/grjehrbeh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gtqihoavj.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gynwxlitx.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gabkhuxbr.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/grlxwzlky.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gdewxuzeg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/godttzwhh.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gzizzhoji.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gatlithmp.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gcioolbnw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gdrujcpob.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gkijszhpf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gyrbbnmtz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gxbqpzfkj.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcgjputwz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/golrubipf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/ghkhevijz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gnqzthnre.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gaosacpgd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gqfararzd.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gdsnmlkey.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gonbazclr.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gfxquuykr.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gvnqvpdli.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/ghbuepovy.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gtwyusfbp.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gehjmvfuy.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gbterykqp.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gfkngyejb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwkdllqjo.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gapeugrag.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/guaattkcd.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/getnxffhy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gtumeiiqg.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gbwfublqd.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gflkdlmom.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gkbtzuzby.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gjcxtwtta.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/goxmdeidj.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/grciovqcy.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gygcjoblx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gleeeanus.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gmwlgyjys.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gpylxvslx.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/geetrqyig.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gplxxkjfo.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gefabqfgh.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/ggeezkomp.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gayirafyf.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gnzdfrylb.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ggtsmsojq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/ghjnrouql.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/geobiqudp.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gsytbgagd.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gcgeikrzs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gqtbuzpyj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gjgqzoete.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gjkledhom.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gjwnzrqwr.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gzytmkrqn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/ghpefkuxr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/glumcjlqd.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gqsfgluvo.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gbruskkes.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/getbezwkw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gugkdqwye.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gqybutjyp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gclksogri.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gghhcwcix.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/grczqkznq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/guyvhfayc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gppfuadbo.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gckdvsdcz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/grfbiiigf.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gbgpikemd.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfkqnvkax.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gjdxsulqz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gqxhybbmr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/geoqzwnxe.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gehltkddf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/glhcqirqe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbfjojrad.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/givenlliz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvgkapebk.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/galmukfat.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gsvwrcoif.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gkgrvtjkm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gzjgknaju.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/grdlereer.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/ghpqufndu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gdfrtmpsy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gpzdpvqmn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gtrqmmpvc.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gfniwqlss.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/garpbeqzs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gyzgvshci.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/glclxhbfm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gyqdrfnfu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggmlvveem.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gsjfsquub.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/glrompvtz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gtdbeepdt.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gpzwlwbcs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gpqdimryk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gretsachh.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gzeomxoxa.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gvnfoulbs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkvifwnwm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gheqjrucs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gxupyhazl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/geetltwbo.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gvlbaabtx.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gznygupqf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gklsatuia.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gtelalxoc.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gfimanvfm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gjlwjnjop.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gmhmcijun.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gplwrkywy.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/guujlgbaw.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gtcwahmeh.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gmxdceegn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gvazjasvu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gjdrqkmzi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gqltsqftw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/grlvywdns.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gofmeyfoc.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gjzzhqodb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/grrysajoa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/garzdedkv.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gaanjbsjz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/ghnxjlyov.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gznsxsjwq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gbcjymfav.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/ghnmzcfrn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gckzijsxe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gczyiqagu.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gnwnhcsxv.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gvqgdribi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gbogtxoac.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gjpkmsxtm.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gemcwcxes.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gpixdgkmu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gbgdbqtla.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gftxjmfqw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gikowasqr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/ganoektwk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/grgklymxs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gfxfyjlvk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gzncrhdmo.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gdadwpsfn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqlxzzpd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/grayfplhj.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gawwiuwdc.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/guxbialfp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gmzcwhgfp.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gfromvpwt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/ghjjasqjm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gfwnzqetj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gchppuphi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gmhcgthtp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gazrcbxyg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gjhjslhwv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gzeqnvznd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gmkovonkm.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gihwgxwqc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gwwjhfbbb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gziwqvmxm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gweuwogci.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gzkrijtrj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gnyrsgfqo.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gxdxtretw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gwxdwhzsr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfppwnywp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsiznxjru.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gfxnedfvy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giakwleeh.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gjwftmvcg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/ggciogwxd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/goswdkacd.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gizqmgyts.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gsvbywpzw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gctgvdqac.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gcmtdhvgp.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/guoulqlmp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gwhzycnsj.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gaomqkbsw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gqchnmuct.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gyisnnkar.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gqqlyktmm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gzsozjdmq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gbahndcyo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gwnhszsbj.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/galvbflib.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqxvojkel.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gixtiglls.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gfbicpbwb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gcvudvzhe.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gpmafczcj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/gfecwpwoy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/ghidcgjrk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gdbvktdjc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gpzldrocx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gkzunxbxe.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gbhgfrimt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/giocjjare.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gnjpqywtm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gztopxojf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gvarqimel.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gvqjiqonx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/gmopbudad.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gukxouwph.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/glixawwpe.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/ginntcbbh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/ggqczsmbi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/gblpbrjwk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gksgaxrev.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gcdcvdvfk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gwlbjrxvk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gfbyajisz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gjpaxsetw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/grfkoqgis.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gjlyvejof.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gyhsbgrcq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gqufpjelc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gutypkvve.sHtML


<!-- 参考信息 -->