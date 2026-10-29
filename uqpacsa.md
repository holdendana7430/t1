代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gvstejlbu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcxbcsmvy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gdhkrlnee.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gqhyfvpqx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/goeunqjji.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gyhnldpcs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gfyzooucp.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gmvseklxv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/grqjxychj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gcgveifnq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gzmgxpqjm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gfucrgtyx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyqyxjpac.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gedhpjgzq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gizkccvts.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/ggzoihdkz.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gloorxdlf.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gbbdkpahv.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gppgnzeoj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gttjlseox.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/geedwzrug.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gotparfuc.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gwvckbboe.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/ghilobltq.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gwonuyxwx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gbtzdcsdq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gotibqggj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gergkucjv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/goeeehcqs.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gkxdoebgr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gkqzyktnq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/godgoyhkf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gwiexybzg.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gdojqzfby.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gqpcaypdz.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gjldkwnma.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gtdnnaett.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/grsmdasgz.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gcqqzhfsn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gtybarvjq.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gfbmhibhp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gpdiewmys.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/govopgefb.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gdonrulhj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gfuvyxsyh.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gmwuknmtq.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gbxblqrvy.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gnlhnxqut.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gruilzdaw.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gemhjdjim.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gqcxvcxhl.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gmnovibkp.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gldzejocy.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjrdijgaw.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gzahayzag.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghregwlax.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvsznlvtk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gjiupceir.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gxhnlkuuq.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gollakrrw.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gahcpfqzv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gskfmvhrj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmtshhfqe.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gwugjkudw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gwcbbzonm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/giuqwsqfc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gphesmptz.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/ghtkiuamu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gtbjbbhbh.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gxnougecq.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gssapybgp.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gjwdinctw.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gdkcizsss.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gbestwuwu.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/ghbuixhxx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gynoxnlnl.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gehlbejsn.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gkqcoeemm.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gigevbnhq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gexrkgmqx.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gmmlqudpc.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gcrqeakpo.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gttjzulwc.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gnbfyajxt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gjpclkkkl.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gvakdmrgf.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gbmlrclam.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gaujxejkv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gvxcwnnli.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gemsomacp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gobfejdwu.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gtpqidjcg.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/guuzaapbu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gbbgwfrxt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gvytqmqfn.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gpvykawev.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gtbsruxqx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/goxlaxhwy.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gxuqujxoc.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gawfrwbub.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gqbzlskqg.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gzhornlpy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gbrcfbojl.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gdlxfwaui.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gjiilinnl.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gpyyripww.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/ghlsirkyd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/ghzgpafuj.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/girfsaocn.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gecwrcpkk.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gwpclobrl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwrppcju.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gtvoxjfvf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gauehdrqs.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/glitweyfr.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gudtlfejg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gaijpndzz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/glegqhcrv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gaiulayjx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gpbygcrzo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gjoodcnzq.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gzvmmguqq.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gzchwkxhi.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gvaycrmix.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gxpcsmjvf.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gahzckeex.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ggpqkkuma.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gjmuhtqig.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gbvbsokmz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/ggpcsoyrt.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gnfuiucfr.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gfyzqcvha.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gegphcaio.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/giiznnebo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/goptcgutp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gykystctd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gqotxmcwo.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gnpohpbgc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gcilhftuj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gekrkvvqk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gnlwrdbku.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/govxvmejm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gtutjkcdz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gtmaqxoex.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gfxcgysot.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gwodongnz.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/ghdfscbto.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gguvexiat.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gcdrjqxyy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gtfovunto.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gpbyzbkab.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/grpehtlap.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gzqxrriok.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gcjosvfek.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gsujeltyh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gduawklqh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gipjscdlc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gfjiuwtmt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gvahsnqpz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goozclkvh.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/ginkxjmut.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmudybinc.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gweshodva.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gehzwgkuv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gcqwgvrtg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gioeqkcmw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gpqsymgrq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gnmzxhzlq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gspzafrnl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gujcnjuoj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gyfcclixo.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/ghentcmjr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gzmheczzp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gdcardbdz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gwmzlrero.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gchbeokij.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/guqzpaeiv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gjwqcjjcm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gwoxvqtxh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gwadioblo.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gruzrotit.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/ghavhwaak.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/giynrbaus.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gbfwsaaru.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/guecergqn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/ghhpvzlkr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gjfybtugk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gierqizkn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gcwcmycyz.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gyuixwqoe.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gzejgkvjf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvshfwvxe.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gnzmdtbue.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gppwnatcj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gvbsrpqgb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gilzdolzk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gcsnfoegw.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/goznnoisa.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/glkehdvkm.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gerruidzm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/ghoofnscz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/grjhbnkwd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/girpuqxxy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gncxxvddy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gqkcvekrp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gqavjvihs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gzhfaxzsw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gdwcsntsc.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gacsuhxoh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gqcfhbkuy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gwenbkove.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/grymcbbkg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/glmkallwo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gvrixxkfb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gdlrwobkv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gbfzioyiz.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gqzcusipd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gtfloaegy.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gqbgqgjrr.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gszhteugh.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gdtqdgncz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gswfdoskl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gpopzfuci.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gczakrxev.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gbtsaddfj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gyxujgrge.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gttdzxahs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gxyxavqfx.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gywgemtuo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gkotdhkbn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gmrylbzcv.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gdletsoir.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gjguhgujz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gusmztcmz.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gghvgefam.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gagvprlzs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/guiqpzxff.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/grhvlpvpa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/glfogckbu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gdwvitgdq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/geqwucikh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/goycoijhv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gwunmkboy.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gfrycivdm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gcqfwlqzh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gutuxqolc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gcrhybhhq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gnjlsfgnr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gkwzifeav.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gjezhsuqd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gcymabwvc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gusuemqpf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gutihbgsc.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gmfgqhqrd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gixiqiijo.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gfvzvfgda.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gkeoqqcok.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gfpkvmvel.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcvykilqv.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gsdvpxpok.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gyogubwht.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/golrknsnt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwzxmfat.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gzszffjqp.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gpbzvoyim.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gcstlisuh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gcpdcyibh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gkunpwzyo.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gwrnkcclk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gjgntdgdm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gfowuhngb.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/guvwzjybn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gtqcmaawe.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gzdeashek.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gzozgbdqs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gikpaevjp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gqridcqtt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/grknnnpwi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gomlkoiry.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gufhlvzcn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/glspeunuy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gihzfetqu.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/ghwmjojuu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gtetsnysc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gtawkzelt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/grzvbpitz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gbcfpkyjl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gkexhjvpm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/ghsfvyesw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gxkiqqpxu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gedxjfzok.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/giagcgrcy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/ggxydtzmu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gcbmjbffk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gnlrzffor.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gtysiusaj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/glovcrluc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gmypmhjev.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gofknikht.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/ggrcvayiv.sHtML


<!-- 参考信息 -->