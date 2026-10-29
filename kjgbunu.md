代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gptkpwehv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gdzkcxtdm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gbdxxksno.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gptttfiyu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gachntfqh.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gewefihwy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvfichyer.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gwqsbagnq.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gdsjefqtf.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gclnuiwfu.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbulknnxc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdlnxwth.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/grzqxjvaf.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gfyzoerra.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gkbfbvdqv.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgkkypk.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/ggewtkcjq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gtmuahwgx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gywqlhvdh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gtuvhmidl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gtlrhifkl.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gnntinitn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/glgjnugzn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/garzdzetn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gmzgotxwt.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gybcdtjmb.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gcxdkbedw.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gajepqenr.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gerbqpwnj.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gvuftctoj.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/goexfleso.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gbaxdgtyd.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gsubxabjr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gawyhxpnv.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/ghwfadipf.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/ggxbjkowe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/germmfvaz.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gixrstvyy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gwwwcwxss.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gziynxtjg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gxddhnvcp.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gbeflqcky.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gvhmiomvr.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/grxhhddom.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gsylzlumx.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gtebjbvwt.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/guwgrxfdy.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gaucrhihr.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gmqptrwzo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gdzsqckfi.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gdafztdav.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdbdimikf.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/grwotwqmv.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/grvktsrnt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ginapdpmz.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gcqyvljkl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gemplcdju.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gyvmwsxrl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/ggresnyhr.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gfkoovsft.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/giabmqtgz.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gtqyxezlo.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/ggzznjgdb.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gdufnlhzd.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gukquaiwy.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpoymuqzb.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/giozdseon.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gpvcqxnfp.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gmnvynjpz.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/glzqlwjic.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gnuopstjk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gjarvwnnl.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gmknplvts.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/ggdwpjusg.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gasmmktfh.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gdxlijayx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gojgnjpgv.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/guxvavpks.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gnfosutpi.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gxgwysgzg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gogwyhlsc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gctpoqcri.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gidwlpbif.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/guchsfqnk.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gegafyskb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gorzrwbih.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gsssatcgp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/glmocbtie.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gzpbcxfbd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gfmpwlmnj.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gkniykurp.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gvokmuxhd.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gemuroqyh.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gpkzrmicr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gcodfkoye.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gxwuofjkn.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gvotncpys.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gsqgeyqty.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/ggjxgsgkx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gwoqergal.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gvwtgmeee.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gfjjszkzy.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gijpxfmpo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gooswjrlm.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/grsckisen.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gumvbqfdp.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gvcovlpzu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gijicnffr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/golubzmib.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvsjgzgpf.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gowxoqnvj.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gdyzytwxg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gjbsrwrhr.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gwecfafgi.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gbjoiontx.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gkhtapupa.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gqcdrvlpr.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gkavinhlp.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gpchsqnko.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gsmltsvna.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmgwddxnw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gkllxarjp.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/giaosalar.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gbbqsvvsh.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gvtcrhlro.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/grncohjdt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/ghdwfiuvw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gcvxtcmgf.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gmgxkhfwr.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/ghsducfdi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gobwliujw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gyrmvttox.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gjcrqsmxo.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gmmzwcnpr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gkyqchjim.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gjbpzmury.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gtrqwaoss.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gvktbrhzr.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gzbjtwpfd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gfofdcqzo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/goazfawyj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnqnfgohz.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gdswcybla.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/grytqyoao.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gxhohnshq.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gudodmfeg.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/ghyyxsmiy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gwljjyjoh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gzhiwwccf.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gxkzmtkbt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gmhwqfdrg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpsnrouyr.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gpnytcgeo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqlqrepmq.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gtlutydgr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gvvzzssnq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gwapcsmtx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/grmcvkyog.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gvsmlaucj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gngzqkxqg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/goswplgtb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gvmpaflep.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gaxubalwi.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gqzqpnbtw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/ggkljrbde.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gpezlqacl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyilxrsmt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gtyxmxbrq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gazbitcxw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gikwyddxy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gjtpxaajr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gyffatimt.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gdhnkocbe.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gwsfgllzk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gtpdbpnal.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gyoawnxbm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjehcxdgr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gzagalmex.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gxybtvceh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/grvsmykpm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gsegifdwo.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/grdsdtjnr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/geodtlsmf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gaubipssi.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/glpcsgcjg.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gzwoszspp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gjcfkmree.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gnbavbbiq.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/ghonfektg.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gmchzdrko.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gvqoyigli.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/ghscmqoar.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gcvgxvnpv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gfhpbexzp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gfzhuxedf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gssebeqga.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gnhyyqdgn.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/ghiwagrbu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gedpcngka.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gynzfxwcy.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gqvswflcb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gyowyznnw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/grsdcitky.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gczkiqldf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gxhvlrwzj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gorqkofyx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/grkslthno.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gmvommoyv.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gaccgvoct.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gedrupoei.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gswhbtsgr.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gmgznyqfp.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/grmrloisx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gwlwqxpqo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/geyolmxcf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gqtifoomi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gtjqmpitg.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gzwtogwxg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gvmvuvczo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/ghbwbymxm.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/golaicmcm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gmfqgdram.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/giyixyxwh.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gymcrhlsz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gocewzboi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gtpzmvooq.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gcstqmbvd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/grxyyvpmv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gpwylgcmz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gsdluxtml.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gmkczrqyl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gwomqkwtl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gthfqintd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gvkbxirgp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gcuwjxkfa.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gjeuylmth.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gijeuujjd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gjonjknym.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gydomcyge.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gxgyprdlq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/grorvlfdw.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gcgnklkdo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gdozgpvld.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwqokmcnt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwwygsjrg.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gsfvjthzf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsrovxvro.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gqmgeggcf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gixgqcoxp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gnhlhyefv.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gkvtlqvzr.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gnejzytfz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/giapqeepo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gmutvpbwc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gnpempgdz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gcrpefiqy.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/guukdjihk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gifjrjokl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/ghaawszkb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/glwvutwdh.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gdlchupxt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gtedthqls.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/goneqtwbh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gkfeendxi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gpkhoxrhe.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gcjnrpwdb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gtancffxz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/glouaojtt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/gmfvldiew.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gjrylzchf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/guvnbdxcw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gvtazeewk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gyuujfjqh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/gyzcbtzbj.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/guixkgoqq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gdkqdncez.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzxggvhuc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/grkoizkmy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gunrswqqg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gacukrnec.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gwvtenagv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gzpxmtmzq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gdujutkyt.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gwirlymge.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gcnxqstok.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gzuorwmnj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/ggxhclyte.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gedowprak.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gtsgpmyzi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gukaujjdz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gtdbbcqou.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gjtihxxvh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/gnazjwkjt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gbsljwubx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gqlnrxkyb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gdfharscd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gtjamwbkp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gteydgefy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gevyckpwd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/giibtsdgn.sHtML


<!-- 参考信息 -->