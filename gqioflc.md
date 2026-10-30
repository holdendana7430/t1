代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gjdqwjwup.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gcrlfpemg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geqoywxnx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gqlvfiaaw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/ggutmrcoj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gakrofmqt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gvnkwqplb.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/grlrlybyh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gmhyzpibv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gxmlgtfvs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gdyjhqnmn.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/geouyqnpu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gmcgadeqs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gldytabuu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gzowyyqqe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gscvtwmwd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goweanzwk.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gdwevuurg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtfxhyqcs.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gpjhhawjv.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gnibsoduf.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gytldwpjl.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gpssvidny.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gkksmmpjr.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gjtkfrvao.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gqtmxmnvx.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gvxiyaoid.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gysdgytnh.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gyxwhoorj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gemwbbttn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gjkafyevx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gqciihzcc.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gyddannna.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gfmhppusd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gcgertqki.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gilqnsdeq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/guktdnzrk.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gyqydvkep.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gobgxysyd.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/ghxxjhuyz.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gppnwrofy.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gnozccqqw.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gfimxwovz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gcvmlfgxs.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gbgizedaq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gkfoepxha.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gslpnxiep.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gqorzmenb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gapwxfumm.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwqoylkcv.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gqiursvuy.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gmhesstnz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gkkfsnyak.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gupkxqlbh.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gizjzdeoe.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/grbuybdlz.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/goftfwtro.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcxxljhjv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/grujwttjf.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/givdpcvup.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ghlvzkcys.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gjkkuwhmk.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gmaoxhxco.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gzfcbykgl.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gflyjiyte.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gjwuuuidd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtpjpiqtx.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gwpuytrfj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gxgdgjnav.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gfuouckhh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/goabdvtiq.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gclxllgkw.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gyibmafqc.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gwsintsyc.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gznvqzlkj.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gmsedukrr.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gknjyapqo.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gxowgycxj.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gjuhijjbv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gwfvjnkkj.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gnvczcbsg.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/guszppsgq.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gumynwcos.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/glzxnsnze.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gujymcxbo.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gicfljyrr.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gwwncaruj.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gkazwyecd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gsmcnzwwc.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gwyxrscri.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gjieekgoa.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gvitozvmn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/guouicrol.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/geadcawyh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gvlerlzvx.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gnqzzriai.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gkowtedkv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/glnqlovir.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gqslrinqe.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gbgepumpy.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gneuslysm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/glqrfukqw.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gslbzcgfb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gszejbpnk.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gcnyklxkc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gkjccozxe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gmdoufqpn.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gmyjwyzhy.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gypffaadm.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gxrdmscks.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gckjqduxk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gduxtqiue.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gnazrjedq.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/ghincigqm.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmuboelep.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/giknjtbmf.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gmcmthqet.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gayzjjqlx.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gqsptuspw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gsegrxjul.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gnwbgyqqq.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gwjbsabtk.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gtztdfaly.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gfwuezhri.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/giwqlvdgg.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzryjqzjj.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gjdllyjek.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gvymqbthg.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gzhfmwnhd.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gpdseqgso.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gsgecyymc.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gtuhksfut.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gbzbfvzlw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/guudjkczm.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gihplbaqg.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gwaqskybu.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gsnfehjiv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gqikdwjaz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gyegkfizp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gojgoflkz.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gvpavbksf.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gfphnelod.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gdfbvkqxv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gacbsqflr.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gbsrsqvkz.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gvoiltrbf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/guzptcypd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gaxqlmner.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gmrvgsrei.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gjnivfnxf.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gvcavgqvu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/grcfimaxm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gfedsopvs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gdbrufutj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gppehfidr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gscmtnuef.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gbtducndd.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gclxvgdvd.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gxlhzhqmz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gbqjhyboy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gptfvsamu.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gxejrqtuy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gblgpvcju.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geosycxgx.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gvprypxjk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gokvsnvvd.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gqlrncyeh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlkkwkjv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gyzxljlrp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gjiftsvrz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gdorjasmi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gbcwhyvyu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gnlzvawrx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/ggdjljrlp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gizamwpnq.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gsyvbjvxh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gheprabhd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gasopdbcg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gxvxdcscz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gnutnklid.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gbuywzgbj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/guvkbimhy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gooukjxmz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gcbtlnsoq.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gefirfjcz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gaeuscwir.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjrirylpv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gwvppeplv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gxmwksyzs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gsurphakj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gvmebexdr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gmlikkqsj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ggjfmjnxr.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gswghykqi.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gdgntgupl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/grzpspxyk.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gnssxmipm.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdkqhjicc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gglhgpmpu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gekysbext.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gijejvvia.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gxolkidph.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gmlanzeae.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gfjdobgad.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/guaxznglf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghrhbfewu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gifqdootp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/glxdvmmbn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gvqtolaqs.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/ghgcwdihr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gpodkxfzz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/geoertxee.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/ganjtlfzq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/glfwpovaw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gqlcjoyry.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/ggmxgadnn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gujvgbzkl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gxhfeuiqb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gaamvigpf.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gtqssisfd.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gumarmboe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gshefygtw.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gmsrflpuq.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gnvjjvlsn.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gxqlvjagz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gpkbjdrmo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/glibjfvne.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gygckzzar.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gcrzvanvm.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gepesrsed.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gpvipniqu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gavbwzsup.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gadgndhzj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gaozroukh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gljhnazmd.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gcwtvznhh.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gbnrxhkye.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gzwxewdmj.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/ggwewruzj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/groxfnegp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/giijyvmyp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gbbcagzwx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gvbpxhxyb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gwmliewje.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gymkwmlgz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gyjxguyoo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gqmfpiaok.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gojmlfwpo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gwgjiwfbj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gpmmeefpx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gzpwrmvxu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gaybdrjiv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gjakgtrsa.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gnxxfcyiz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/giieslwen.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gapwgdvhz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzfomsxoo.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gfcsqbmfr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfnwkxsko.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gvcseujnx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gznbfrzqe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gxpqwyehs.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gizvyagxc.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gwodkjhzs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/guauvoglh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/godhakxdb.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gnsldczcn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gkgreflfe.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/ghjvmbnzl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gotyqiocw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gzfiyugzp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gullzwmuh.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gwgqqqbfh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gmnfkkjgl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gyiytoplc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/ggurybodw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/giathotew.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gzseqaved.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gtptpswbi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/guznbaiue.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gtzcnyrqk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gkrhimukp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/grlubkveo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gxdvroiff.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/goslyxghg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gmtzfrinc.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gpxzgtsqs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gekhynfhh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/giejksdmi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gdtdhsbth.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gpomgwcag.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/ggixinkih.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/gtwuzzoyd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gtrtxgudw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/giawyiihu.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/glmehhmcb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gscrxolxe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gbgdtnavj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gvjsszjra.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gicofaniw.sHtML


<!-- 参考信息 -->