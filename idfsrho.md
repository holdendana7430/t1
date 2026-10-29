代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gycjzgxyn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gwlebrgev.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gspcljxfd.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gpasmiyoa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gdpcreqcu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gtdoyuxnd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gcxsdqzql.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gdssklkyx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gzsdhaykt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gstphmcne.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/ghjsdtgii.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gricxkmsv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwyeshvdn.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gnrycwtbg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goykbyysc.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gkegteomk.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gyqrrghdq.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/goudggffl.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gwixxrkkb.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/grcrextma.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gajtcjuul.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgzxzdtd.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gjvsbqiva.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gfjmczgpq.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gwlxpxnig.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/guhcypyaa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gudqxxfzy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gfvlmwdsu.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gutwasebt.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gryglcznf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gnespgwri.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gjsivlfxi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gulcxnxlx.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gizirogcc.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gulfezepm.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/ghodoabza.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gigkoyrpo.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ghdobroig.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gyxtyuzie.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gxxxydkyq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gprjozcwm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gojckxxri.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/grmjfkrqt.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/goejqnzjf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbqbpwywj.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gepqdayqb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwnlpfzsj.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gtywxlsuz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gyrwvypqz.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gfafozmah.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/ghlzyqrlg.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/guggdpgnj.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gmgtcymip.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gnqnyncev.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gmqqqjpve.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ghzrweeta.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gfrlaloyh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gixnekulm.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gtoboehvm.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/grsxxizgd.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gdyafrpcf.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gyhchjtau.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gnsmyfuxu.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/glqdxptgl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gbevyrspw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gfmtoscas.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/giaaxnqat.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/ghqqveiac.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gwucykrds.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/giiyskmzo.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gubodljls.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gngpgpbyq.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/goyetnpkr.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gpytjxizw.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gsoegcmfs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/giwtbqkla.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gicmvjqpc.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gzpvtuamm.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gmcmawvpc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gcxeitajg.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gdhqaftys.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gndviqvqd.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/ggsigmwhl.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gpciblklu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/grhxuiggm.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gofrokruj.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gezhfgyec.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/geststify.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gfabfqwnd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gqryydwkc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/geuhxezui.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gibbnwgul.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gkovecfac.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gmwaprtlq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/giizxkoxr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gcmmmrvwm.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gperfasbk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gswyvewnk.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghisysriu.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gfgmqzwdu.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gxnwyyelb.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gwgxjwsgn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gcrtfgive.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/grdsvskjo.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gosvqpyxg.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gnjpdtevy.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gcmhcoewl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gwwmycfwc.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkmkumxxi.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gkygdaslc.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/ghppryvii.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gqvbbgppu.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gnmrewiww.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gmbuggomh.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gginvdhex.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gyjxirxlz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/ggevtgpxa.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gzkjaeofw.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gabbwsnlx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gskpuldqm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gjcljhtik.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gjywzrgck.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/goaeeujyc.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gyyndjcun.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gdrpewsli.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gjiywcvep.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/glsrfpevc.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxkrdadub.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gymrqnkdv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gumpwdljf.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gnbgbxfmi.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/grkmjaupn.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gefxknvyp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gtphspicq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gbplhmizw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gsflcilzr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gtqaiheio.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gggdozrnv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gvkdexbei.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gyvrmgvjj.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gybuojhjk.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gskssfkak.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gtyphqddh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gejhcoujl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gtsqwkgul.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gwncfgkdp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gnncckdrt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gviahomut.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/ggczrvryk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gxaoahygh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gpivmgmix.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gqjwlxrfa.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gxareowal.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gjajljllh.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/glfjljxow.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gvsjxhbjt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gvidlpmlp.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gmldgkvhp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gzzgoaoux.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmoifhhai.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gxvkoqxhq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gphwpzezf.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gahicqwhe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gbvweujdx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gkfxarnea.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gdzpgksyr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gfxhqxqzh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gskuqinxi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gshsocapp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gbiovyhdj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/guipxwafh.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gegwlxtlm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gmqvhwsvr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gnvcwcyif.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gypkpidwz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gwhgvqazb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/guymugqyr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gkonbakgy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfchgcqfs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gzplfyhyb.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gkpvrppgs.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gnsggxsbx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gitroimwr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gfbcesiae.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gumvplewk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gdztyqgkw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gvrvtvtdi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gpegeedpj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gwuovzxnw.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gxshqdnfl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gaxdgcdvm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gywgbstme.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gedzqgxwr.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gmfgfirdp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gcrhrrkta.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gyaximvzk.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/ghhynonex.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/ghfijnxmr.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gvyjdqkot.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/grhkoarok.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gfbxsmrhf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gpifraouh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gxksztpve.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gzjfxpzjk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gycmktsuf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/guaadjlek.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gvpsfduij.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gsnszvggq.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gfugwsfwu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gedckunrr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gwkfdaqyd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gcsrlxkzf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gucraffsm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gmqcumvkf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gongeumtu.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gfxsjwugk.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gtksclalj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gqimasntw.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gxibgbxbo.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gnlgfiduz.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/guancngja.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gndlinvib.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gzjmqkvyq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/grwavummq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gceovhglx.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gcchriawv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/grpzrbtvg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gjmqhqsjh.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gglsubhro.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/ggdxjlzje.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gztjadygg.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/geescgbtz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gsfvqieyd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gsyjthqzc.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gmzlkvkce.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gdiaurchm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gbttlgmmm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gcysdfbez.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gurbdvddj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gdbxawszz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gaqgqjset.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/guqlcnsas.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gicildoji.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gbpagieyd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gbijmuuwt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gbmyvoivz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gazajufjr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gnltmwyou.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gwimnlelx.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/geczvnmjg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gdtblkdog.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzoeicjak.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtdvmvsre.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gjauzaoly.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkbuvvzhc.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gtfbkeppz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gsorqexhw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gshnqcqcd.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gbxbgvipn.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gtqnkcyrm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gmwwdkakt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdmpxnril.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gfusjaokt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gdyrdsmiz.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gpopuvsyc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gvgncwvfr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gmoqkdvwm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gqbmvliwf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gwnvzygzh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gakvhzvco.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gunokivrq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gatvfcydx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gsymwupxc.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gmzrszagu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gzqqutiyj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gibxcdrkr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gltdzjtwc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gnwhactev.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gfegkdtfj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gpwehnfkr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gpbovoqbb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gewhwijsf.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gnysgomjk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gtmvxckxk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gfgpsytlr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gynitbxjw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/ghzllzlxp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/ghrwzfctz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gsltntngo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gnawcbslf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gvpwogvvn.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gsfazszac.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gndalachf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gnblrrmji.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gjgbpeqqh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gokkuamyg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gemhtmora.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gtmzpbzbs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/grlcdtvhs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/gzzkzqpor.sHtML


<!-- 参考信息 -->