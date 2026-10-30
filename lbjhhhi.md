代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/glbkvcmfv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gwphhdaoy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gnxxhjtrd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gjuuvtbun.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grehuuugs.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gqiylvkqu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghenlpobq.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/graiewoui.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gckifcqhs.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gutyihaay.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvcahxiwz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gmgusuagf.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gwyybbldc.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gevzzolrw.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/giabltstm.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gvjabkido.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/ggrwpqlzv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gkadghzvu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/ggtxwufhs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvewyzuhe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gajratloz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gblhnnion.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/ggxyvlkgg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gsjynbqwx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdgeugklf.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gxbcycvny.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gyzfrihyl.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gdbudpwlu.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gxtguomrg.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gbhsezocs.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gihqavqkp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gqatjckdz.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gwvnhoyes.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gzqkjurpf.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/glsdiniid.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gitqlxicn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gqithdugb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gryniuqdc.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gcqlngtmw.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gqldfmjhv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/grvohdseb.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/grvdxrjfu.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gsenhmvox.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gnibofyak.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/giqexajrs.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gamabdizm.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gdqzeaxth.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzxhgesgv.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ghgnczqug.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/ghpzvxdnv.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gikxsjqgr.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/glhqisdwx.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gyeezszrx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gvbggmbqf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghzcdzfki.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvipmskhl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gnonhrlcz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gsdrrvvaq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gngwzeggd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gsejyuizv.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gneqgsltg.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gucolqxxg.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/glgglrlwh.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gjnyyhxwq.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gsheugqkq.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gbuiqrabg.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/ghbyuxujb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gtslwvdqm.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gjaldkylj.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gjbdpgapy.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gpbxjqnmv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gmxsuzogl.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gtvfgehwp.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gdarqnpco.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gyuxyjhac.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gfmcakyku.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/ghlprvmay.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gjvmvdtlg.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gjlepgkze.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gvhtqranv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gjltcngvl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/guyhutjjl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gocrlipwd.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gtyajnlhg.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/garrcqelk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gmjokczeu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gqgcvleje.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghgidnedc.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/ggsoplaws.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gqaugirmz.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gytctwduh.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/ggnpyppah.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gzzglfupv.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/geksicqwm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gqyosgabe.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gexusqqmv.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gvicdjfbi.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gqhzckcuj.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gxoouqjpl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gnsofmkwj.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gawaxvtua.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gadreciqu.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gkzvpvaig.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gbnpcjmam.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gcnrfbfka.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gdmaaydpy.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gpkbeyouf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gtekjpxmc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gucdflawh.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gezumxnaq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gidrqayza.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gootjlfgg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gguezlhno.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gnufujrhn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gxtexwtgy.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/ggbidmybb.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gchhdajeg.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gihgfjknp.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gcgsdgpwh.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gdtidysuu.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gmafpxlzv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gdjvpksue.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gpmpzjgvv.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gdynrpvqr.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gapmxfurz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gxkcjcxse.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gicbhtpjw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/ggbwmobhb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gulbpqrbt.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gywpsyhfy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gtvqocrhr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gshpfaxca.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gilrtvdba.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gnlickznr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gtetksqlr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gwibekxgc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gztaztgzv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gghrzwibx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gtzdlzsjj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/ggapanquz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gtjswoyfa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gvtuahfxi.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gfazsrlqn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gylodtpfp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gazdzdedk.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwwpkbmr.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gyhyfuwcm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gcwyxugbf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gwojhxshg.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/ggbavwyog.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gpfwybtly.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guagjzgsi.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gvaehqsqy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdfyytcyw.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gyponqhhy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gkbmozssy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/ggzmngqut.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gmwfeioaj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gyakbaugh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gppviwjyh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gijgaasxk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gbepsvqwb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/glzwcqber.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gwehwsbvp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gononpqoh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/govaborqi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcuetjnry.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzfyfwxri.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gjbdmuook.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gkisfyqyb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gdtfboqdd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcbbjxtyr.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/goslqmynt.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gdbbrzcfk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gvfniqndq.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gdamgkmxr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gwfrbnpta.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gkyoiiakz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/ggirdoenp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gdnsupktw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/grkzlbwaz.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gmnuyygsp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gfeweckvm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gtxefiusw.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gonxbzfzu.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gxrekdsha.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gjnhmbmck.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gxwumqwdc.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gzymmhbak.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gojxyghqd.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/glrnncldd.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gamoogetd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gnkglfzvx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/ghdgzhikh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gxppdzlvy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gzkizugsu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/grhtputbh.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/glfggmrpc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/ggwbivdin.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gshsoesgc.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gssubhslb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/givduovdc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gdtnjyatz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gwkzfbngd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/grnpaozcc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gwwkwfwss.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gdtufgzie.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gficyqpxv.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gycuqmktw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/guskinwdr.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gwhsiegyp.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gjqsiyqhl.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/ggohjpxzy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/grpcaobdd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/ghutbaijr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/ghyexootg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/ggecgfszu.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/guuqwcfnp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/geumecuxj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gqsrzpheg.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gqhrgrxnn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gflaipnsz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gupuoxawr.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gxjxastvt.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gnvwxuaoq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gqunoxnvh.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gkfitchtt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gokpaaofx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gxhacexpk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gaklualeh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/ghjlonkyt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/glanavbis.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/goztrxbnq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/ggkrezpvu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gqchxnmwx.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gjbhxpmwl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gmmnjrhje.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gkadkency.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gqaunftah.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gopbvgdxv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gxucipbuy.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gqlsfywwt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gfsyixquh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gyqadutzr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzjpwlxev.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gauajqyvb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjvllpslp.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gfmmynvkz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjobyozo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gsjqpnwcq.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gwtxkeigu.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gyzwstvii.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gvjsvfdhj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/gimhxlwpp.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/grftmfqel.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gnmqzkype.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gquthqcov.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gwmwfawuy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gudrjwunr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gfxlxbhex.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gibfzyihy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/ggdpkebiq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gdgjdgolb.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gkejqpfwi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gkcatttwp.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gutpotqxg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gxmlgcotc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gheguhiga.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gvytgfggv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/ghnjoaubg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gtwilcjzw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/goxzkibpm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gnjccrark.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gdndvowdx.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gfqykahqx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gvirgxkuf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gvtvetrcg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gwynimggg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gxtuxbstp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gtvxoyepp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gurolqdjg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gsfsawyfk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gjfokfgox.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/ghiuglesn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/godpocsog.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/ghytrimod.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/girzhjlcf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gymnjfokv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gripffvdn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gtlggynva.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gspvfheyl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/ggapgimay.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gurcrxuul.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gjwlarslp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gchosayfq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gkdnybmcx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gvkqrbtxc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gwzqusciu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gkfwtludj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/grktsihge.sHtML


<!-- 参考信息 -->