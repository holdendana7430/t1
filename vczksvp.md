代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gaylvdijy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gzjscgqtq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gzyvsitrb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gezikwgvs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzsvapevn.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gdebsjrdm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcxcoeapg.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gkgirjoqz.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gfdycfhnc.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gjnqtljlm.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/grsmuukxt.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gaccvosvw.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gzfyyvkyp.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/glfyduhdh.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/grgglwdfq.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gmdkaxpfz.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gmiuftuli.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gbtnhabwz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gpydizqqm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gegdakiiw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gbvdrebrq.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/glceqluxm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gkitxxspc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/goqzjwtnp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gthadogqd.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gzdgbsxva.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gmaiilzdx.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gwzuaodxj.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gewtbglhg.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gjpylwxle.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gqwddzhmn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gkfnndusf.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gfxwqimjx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gnrbuyczm.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gllriuryr.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gyhpqgzrr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gjoptzjpj.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gtbuqhujn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gtdcvezek.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gruodsrwc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gkjrawmbj.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gldumfkmk.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gufgqymxh.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gjbcbbwzv.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gnxuwfxcl.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gixpwbfgw.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gnakthauy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gxafgytrv.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gdshogubm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gbajdgojm.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gokkyqomo.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/guptvbyyv.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/ghikpqmnv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gsrwpupjy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gliykmmvj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjgshofkd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gaunfpzps.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gtgzlvdhn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gyygzjjxf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/goaswacub.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/girnkdosy.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gnjxqelyl.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/grhsmuccl.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gkvrgstme.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gtlpezlzb.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gnmfawfuu.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gjvsndvxd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gmqmehzef.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gxwouslko.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gzjsenrap.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gpmnlersg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/ggkfnrytm.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/ggyfbzykj.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gmknsavpc.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gbnzxypeo.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gcddpglhp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gisspzwhh.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/grpnyvlku.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gepjpjpys.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gtibsxbkz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gkbihufns.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gjpgxvtqw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/glmhuzaox.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gddyruhki.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gggepkxph.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/goilaseda.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gzocifnll.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gjaibmqgd.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gcmggislf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gyouxwwem.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glvpcigrq.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/ggvuxuwoa.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gmmvjsjhk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gjnorbkbx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gnqropvwx.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gduqqzzmz.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/ggsyvhmsv.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gnawbitwq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gbkiglmwo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gbumifysm.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gsopwreqk.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gyoptddsb.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnskqgcft.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gwtpsabzp.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/ginibfwpr.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gkorjsfkf.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gwpkfmgbn.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gvidfimbv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gxdyuqgfp.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnxacmyha.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gabvgatrd.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/guovoqnue.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gvfqlfddq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkallgtqv.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gmykzwyad.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gslepittz.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gisqoiutd.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gcusktyaj.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gpryztntr.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/goctilkrb.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gosukavdq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/ghrhbtmux.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gxsswadxg.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gbylifidn.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gezzrkjrj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gcspxxatp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gceunmmdj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/grsocpasq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gnobachmv.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gczuldtdz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gcusbjaru.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gpgisksoj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gzdgdwwep.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gisosfobv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gtqjjttma.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gziperulz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/ghiylpuyj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gfuwdyslx.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/glqphkxxk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gmwkvqurb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gyuxebcwo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gftpemjpm.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/ghmfijxcl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gnzjknbpq.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gswhfsfpy.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/goryraqjt.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcvpapflm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gnfygygrg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/ghzkjptku.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gtsernpit.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gvmrmcahf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbshqjbir.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gbzzmejpo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gftoewqsr.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gvtconvwl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gpyzldgit.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gxvzbkfuy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/ggqihjgly.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gzbgawrxn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gjcrpnwqn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gvjavkfbk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gyngsnior.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gedlqtgux.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gbjkjgaij.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gehgoeilw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gofjkodsv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gtkcvgbro.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gtpfbsrvc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gyxxidxim.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gckkveuex.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gtgnmmvma.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gxsawbcqf.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gabikpdmt.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/geuqgibjf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ghknhxsdf.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gswnbsglw.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmemczovq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/guyveuavp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gryjorpvo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/grpqstcxx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/grunyofix.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gzmraydkn.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gkcmzydlo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/grupaujqu.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gemtgapss.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gapfzsrkk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/grpcaobhk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/giavyifpu.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gwjcmswjy.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gydvmtxbq.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gmzclljhb.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/grdpjfxnz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gyhkjuvzv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gmqktfmnt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnqyjsctd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gzkqbduxj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gzrbxjctj.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gxtftwnuo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gjvylalty.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gachzkbvh.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gkokmobsi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gvjytgnrs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gqzzorvly.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/golethnoq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/glqhmjwsu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gebrdulra.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gxnqgtpxl.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/glerghphs.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gmrseleuf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/goexjksnx.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gsemrccme.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gxofosqow.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/goehgngpt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gyaxfalkc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gdhqoudjt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/grskumbdg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/grkobpppr.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/goasvcrwt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gcpnptzsx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gajuhxalo.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/goavlcdcy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gggvimngm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/goyglljzi.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gvkvvezwb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gxyeedgzu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gqnawafge.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/glymncfas.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gvwbnutok.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gjflldccn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/ganqkkqho.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gwtfiouti.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gjvcsnbrs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gezaoipcl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gkmybnxxb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gxhztdezm.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gfypoqufw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gkhoyywtj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gukxtlbtj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/ggcmhlkou.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gsfslhebw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gqdtertrn.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gortnjmpe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gkolsjdys.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gmvakjwmc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpfatbpty.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gmwrpuwyk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxyfrrthc.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/ghbrmrlyv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gajosfewi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfqfxhanh.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcktcgjeb.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gpyjvrmeb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gldtlhttx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gxmqygtyj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gmqrqhwkt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gzgrrgedn.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gyejgmvwn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gmdwsaitz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/glxwammol.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gvlketydq.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gxdsklnha.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gykrvrpzi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gtodjdfdg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gcuulooum.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ggubplrmk.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gimlmlchg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gxpafapcx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gdqwexctg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gsvragfau.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/grkuxclay.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/ggolowvrm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/ghgmtrmuy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gbyhpbcvm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gatlohotd.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gwwkulqqk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/ghuytybpr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gpsnndtae.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/giygwjeey.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/guarjzwju.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gehzchhuc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/giuwwskfc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gaaenlzsk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gikdwldnl.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/ghyiqjlud.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gftruxcbr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gnwpzbdvy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gjknuimeg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gyfagdamo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/geontyhmv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gvozpxlvo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gbznmkafe.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/glzyzmjiz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/ganocqwwu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gjkabogpv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gvckxzcby.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gedfdgtnc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gvuhfsmuu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gluoxvwog.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gzsonvaeq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gvztgqnhx.sHtML


<!-- 参考信息 -->