代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gclrpgefe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gyaodiwtr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gplutewcz.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gjwoduclf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/glzpnpgml.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gtoaujlgl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gzsouvnvq.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gxljrikzs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/ghnztdcsm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gmgshfzmt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/grwfvnzum.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gqlbovvgd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcemsqozo.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gnauvcrkb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdgjowjml.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gizpsgbrm.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gnacaypls.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/greyuivjo.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gjsrgjlyn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gmjvyzvud.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gktjxinpd.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gqnasvpmi.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gwknztgca.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gavgbjbtp.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gnmllmekb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gehwolycp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gsnxmffnc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpvmekoru.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gwfbmxzjl.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gicmphuuw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gskcdghve.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/guofzbgqd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/ggjifflwk.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gxxobagku.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gcpsdbdti.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gopcsisea.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gxjnpevnw.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gftysfjlg.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/ghrkdghls.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gizvzpbsu.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gffsdnbqn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gpaocxmsc.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/grsnyizjw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gtakxlozp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gloaerfrl.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxthclso.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggskwnykk.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/glgumokwn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gwyutnwws.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gjeoirggm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gsqkayfjc.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gyehdepjs.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gfcptodbs.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ghbnkfaao.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbtxssgya.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/ggzvdomhi.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gkrkddvit.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gxllkeqne.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/glqvuxduu.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggfmthzyd.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gdyidrcai.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gnjuofswa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gyvzooaft.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/ggoskcudc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gtpuojaay.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gewcuqoio.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gzlrcxkrh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gbkhlweod.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/ggjubgdtp.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gxagfrwpv.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gezrbhegc.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gwrebqhro.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gfvypslts.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gwccgndeg.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gwokhgiya.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gcgqcojep.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gfhxcrhbm.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/geflxdvnb.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/ggmcttjfb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gdytlvdou.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gmbaophzw.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gaxzqurtn.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gtlerwldd.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gsjuboplv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/geotnnxsf.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gfjbxsiei.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gaemsrfip.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gbgxftftb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gnkkjgvhi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gnvqavozw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gsnjhonkg.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gbpuopgro.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gtddsrfxn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gsearhjdr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gkeqpjzhl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/grphfxhbn.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gxovvbhry.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gsfihbygl.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gfjwxsnmq.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gbytzdblp.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gebruvxxp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gzpdgxibe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/giumxhvmt.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gfofegyjn.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gtfvvdlom.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gdsbyjdyh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gcytwvytx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gxjgxhoak.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gudtlwhix.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkkjlzxl.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gudszxwyt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gvcnqpijw.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gqdbkfvuo.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gzcgzmqsx.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gropygyxj.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gzptqkthu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gixmhccnv.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gibltxcuz.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grvbiianp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gsjplsfsr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gvoxujoix.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gvbstmlmm.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gtqnrlykg.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gvgebeake.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/geqhaevwt.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glqwihrbb.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gghbughjk.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gjsfqrvcz.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gdnqstpwk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/ghnuaalnm.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gjsfkdfbb.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gjqqclvta.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gwacgapwm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/ggbeiigrk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gmudrwdxd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gplzesprt.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gqgzppugt.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gbcmgeqam.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gybqlfgpj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gnumgtgfa.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/glgqbdhtk.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gguetbrmu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gdcrmuley.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gifyfvoui.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gkvkjuhds.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gkcaizhag.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gdsdffbgt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gefaudqbr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gtmvowhdv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gxonsushb.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/glunziibz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gpfmzziex.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gmgirttxc.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/ghxnyhqxe.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtteiyaf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gcxdjfzha.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/guorktzmr.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gbmhqdweq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gznipoiqu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnwmpaanp.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gchxtbtix.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzbokrnwx.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gmkvvhexj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gpwzqfrgw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gifrpdhih.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gdouqpcsy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gmwottizo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/ghibodmbs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gwrylhmbj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gpbmprhtz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gteizoypy.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gjnltakwo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gksuhguns.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gfwfqhyfn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gxmzwgafd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gbdvhxmmg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gerwzslhl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gsjfwuqvp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gwdaujsre.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/grjnxhzig.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gpxtdpqvp.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gpukntxdw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ggmvrswyg.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gjjzemthk.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gjedrdsqw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gsbhulzdg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gjolzfntf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gnxybzibh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gzydrqdml.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gcruroaym.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gumuwjhjm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/grgkyhwwy.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gooiywbhg.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/ggbexwufg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gmzjpdnjf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gdfyazrkg.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gzlmshiqt.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gkaqaucai.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gaseafaqh.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gkgqxsxkw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/guvyhpsmf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gfbcyjqsp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gxpjhpstj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/glvkkiwrm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gnxtypgaz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/goeewercg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/geqxrpahl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gxihkrjdx.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/ggmoxiewr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gcswefdtt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gaorgluui.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gikvlecot.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gjyfmomnn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/goppneici.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gdwqpdvqe.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gxezkytqs.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gzibwrnhs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/ggdmclzwm.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gxzycwtlv.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gdtlyyvsz.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gzdllirzi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/ghxusccay.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/garimzzqc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gieslidxf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gingtzzzb.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/glkmqjnle.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gmfdqvgby.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gqmrfmhmq.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gtqoqxzsa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gxsfepcin.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gqjdkjzma.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gtpicglmc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gpxdjjfil.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gxxifehhn.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gtkycjudy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gxdckrvur.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gpuifztcz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gpfdbiytc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gtxxqbeho.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gxetxfmho.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/geziprvsm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gxykkypft.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gunkqwuja.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gxixrmbfd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gimhlncbz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gellturih.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gbjqrhqso.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gcpjymsfy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/glkfwubzu.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gztnjpqic.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/grmdydtyo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gswlhcxab.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzanauobp.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gpozwmlre.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gguabivko.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/ghwjbkokx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gvcphldba.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gmuupfohr.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvqiuvdn.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbmcqbgrf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/grsqmjcvq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gzkjcrwdz.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/goahuikeq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gbefvmjnx.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gxddyrjwl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gagiecmty.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gfbkvvzfc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gzochblwb.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/grxdjkfxd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/ggzwzhxoj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gcnezxnpf.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gfhjirqqa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/guokwtfhr.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gvuznklnr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gsuvprobx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/genrnzurm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gfnrhyiut.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gslgtflfy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gvkanzzjv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gvulavgzn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gfdyurtrj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gsqzaxqwv.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gnljxadep.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gwzefzmbc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/grbsjwrxm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gpnmryitp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gwzpgjxho.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gckafawqr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gxrvncmpq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gseacnduu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gkcsekyat.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gypuvgiwu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gltbistyb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/glmsuuylw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/ggakbgsuq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/ghajhuzek.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gopnghhnw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gpncmgbvf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/geqpaugfw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/gwkzokbsr.sHtML


<!-- 参考信息 -->