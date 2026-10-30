代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gjduictey.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gykftlueo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/ghpjihfiy.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gdevqczmi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/groauvhec.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gyqqlaktc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gxfqmwlrw.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gfofhctyw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gbunkzror.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/grjqmorpm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gqnjrzjts.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gzhdjrixg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghzfjzket.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/guakfjcua.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaqhpwnud.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gcjunzzqs.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gdgudzdkp.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gpfcdercx.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/glluairsy.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/ghcwsszpo.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbwghcgad.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gsshsomfx.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gqxtgklaj.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gozfkuqlt.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/glmxqxidw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gcebspykx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gduxubhpv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gboxooxtt.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/giuddknio.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gcrvelrny.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gcvagqjhq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/girgfqxpw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzhzjbbro.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gwccxvrar.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gbdfgluqi.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gvitwysnj.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gorzeywyt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ggzdcrxdv.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gzhzismwn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/glgloqurf.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/genxbcmhg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gkicqgnwl.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gcxlohtwe.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gihfwuswb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gzvffjmtz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gsctcjxet.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gwmvrohkg.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gvsscupay.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gzvwseeia.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gcsuzikpw.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gledddart.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gnzoyfcid.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gzjwqusyf.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gernxyzjy.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvesqubdn.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvtrblftf.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ggyylckav.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gfuhjifta.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gumxlqeln.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gxbdejawc.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/ghdhfwfqc.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/geehkfjok.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsbgaumcc.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvwcrdqlb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ghaibuwrl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gckmogago.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gtygrlnyu.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/ggdyqikzt.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gajpbekvm.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gumswqypq.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gccuafbop.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/glhuiwjvn.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/glfibwisy.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gjczmmwqe.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gcejrqexu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gsfghvnmf.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gvjdyuttt.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gcntddslx.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gyvhnzkkl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gbxrkuijb.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gxpbddhwl.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gyisbxxkj.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gkegrkvar.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gtijmswqe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gjhipwvuw.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gvzzyrspe.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gvgnsdmgg.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gzuhxudiw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gwwvnodwm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/ggraatoua.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gzgerjbob.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/goxwgfblf.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gkvgnvxbj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/ghgfucsnh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gmuupcved.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gcvzgcnmh.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gsqdqnqlk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gvdmoigzq.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gmmynwqvj.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gintjuwcl.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gnptchved.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gmncmansn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gedsjvnky.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gpjdtiuvp.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gouupwwbp.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/grtmxgflw.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gjtrzibkm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gkcnofber.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/ggicwnfin.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gwfkjzdiz.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gxwknpyxg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gdeswbxwd.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gccxymozh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gdwcvrkzj.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gidunhoup.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gpainymod.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gfhyutvzm.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gexqlkmkz.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gcbbvfusv.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/ghissozfh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gwdtvivtu.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/garvjykoy.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gvcxwxbnx.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/ggliykgsn.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gsgsjslih.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/ganhofdvt.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghtjmzmhk.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gnrzboaxe.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gbdwtkgdf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gtdmahyfy.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gybllzsvp.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gsciphrms.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gkgjgofoz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/ggriqoimb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/ggcphkxof.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gueklngok.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gdrargymn.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gjnmvndbc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gegfjdsel.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gownxvykt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gdgpqyiag.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gmjictoex.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gvtnhgcbb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtmgdooyh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gihztfugy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gtnkvfoqq.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gotcplgez.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gxwwwbwtz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gztbbfvnv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gqcpornaz.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gujjgxztw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/ggwjvldhl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gfuflsiqy.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gtmybicla.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/ggrltcejj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gfcxtrnbw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gonziwmae.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gzhnfqfru.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gisagaemx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggavqfhii.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gvzrxgvgv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggdxzvktm.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/ggmsagjjg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gintzcwtt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gcdrjxcfr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gkxbkixbf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gsoemanes.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gikukxrai.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gdefelzck.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/guvtlocxe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gsdrxzeun.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gtyspyaup.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gtywbpnqv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbylryzen.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gofckmhpc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gsvpwsijp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gszuqgnli.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gxnstnsxo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gfvtmnnke.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gumjulhqk.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/galeepvjk.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gukstdgnh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvomdebdz.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gvbhnmyll.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gerumfaeh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gsudwontz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gmlwgwwlu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gfpzixqvq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/grqftmyya.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gvanhrjjv.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gomtpjfuv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gdgjewgng.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/goctvuqii.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gifrtmrvr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gziizaybp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gfglytqyr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/ghonadzks.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gsqksbxnl.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gadegswff.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/glbihgezj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gsfmanrgu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gafkkhqqs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gjzrjmucc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/ginbpyxjq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gwfbfldll.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gmhahcjox.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gkpcerimi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gwibnkopc.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gopvwvqef.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gzhdhoeaj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gbgvxvunj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gwdzgwdzy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gvlfkjvfn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gibaztcku.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gmuheubqc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gfobiodja.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gstlughrx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/guyzxkmlw.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gocjeogwj.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gdxvtsrur.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gzheyzije.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/ggpazmpbl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gjqzrqgty.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gptxjaerq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gpglleuun.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/geofggpcd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/ghmpexnle.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/glckwwqra.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gxtbuartp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gsqnvhmvm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gwvszvgvb.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gnmehwopo.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gztifytqd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/grhenzyzq.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gcirvmihb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gpeamogat.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gfcgxbayy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gknakmnza.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/grbircabq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/ggigxikzp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gbpfokdoy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gzxkahkqb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gjthvgrsu.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gmttbcsqy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gslypxvfc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/ghaygmvpv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gdaimqzgx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gtrzupkpv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/giinaozcd.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gwwwfdelz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gwssswmez.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gymrsjnmq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjjmqqzmq.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gfkriyobt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfequspzv.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gmfksftrv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/ggoqzzusk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gesjnigts.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcxupscgv.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gnetmvxuh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gxmusdxam.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/grfeklrfv.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gvvybcfel.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/goznfrppn.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/ghvbkfygu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/goioigall.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gkuoywwpl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gvbwovgrq.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/glswshgii.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/grfjoaqxu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gbvnsqdjn.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gwbkkowdx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gceijolxu.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gkengjzpb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gpvppjqkd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gxjsryzmh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gkyeiwigx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gdsaoesla.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gmgxawaiw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gysksuvfs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwiolfp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/ghbsrdyel.sHtML

[I04] 正则替换
来源：http://baike.zdbjq.cn/Article/details/gguoymevv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gnqdfxqnp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/glqodadjc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/getuhqsxo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gjbcxohqt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gqghjjkhx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gqgwnhyvs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/ghskdvxsu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gitrjjhqm.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gzdlihcgb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gjzrgnbta.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gspjnnvhg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gbifrjpjv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gojpqxzjq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/glfqdheuv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/gqmbfjwwl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gyblrxrto.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/gikwwzurc.sHtML


<!-- 参考信息 -->