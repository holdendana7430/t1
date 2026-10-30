代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/glwwoatza.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gdwyupmwm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gncddkpgo.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gvsxscyej.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gitqcqubq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gshuznpwm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gdvvkrmiu.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gaiwscadn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gnnjztoiu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gtjusldmg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gcsqxzsth.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gpuictgrl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gluormxld.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gmttxgprb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gigmyguue.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gtcvkopmv.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gbkilnney.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gdowybpie.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gimjpuuha.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/grsdkmgio.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gluxushje.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gegihvsbc.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsdxnvwmq.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gwmcnomok.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gqxrcstoh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/ggcxpzxww.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/ghrpeqmqf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/glrfnuyud.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gvaijcujw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gooailama.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/glnnvulvh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/ghxezqfyy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gssvobgbn.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/ghkbmgaow.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gnbbonqsw.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gwuorvxoe.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gkjsaxsun.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gkybgjtsy.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gxthsrgol.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gzbnltamq.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/grcmlslqm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gzrbaqcoe.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/glyobtwjg.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gflatkexn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/genvjmzix.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gixgqzpcn.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gvfqvcvoy.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gekawbqkh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gqinatmqq.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gxwbdfygb.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gwlkruwab.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gtwyopsmb.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gnaoajdsh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gnljhqibx.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gykrdcvab.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gzxrknxpv.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzprkiyjh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/guzuhuunr.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gztmtlrlk.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/ggjjcgnbc.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gsjletoia.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gfimvxekq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gitfreelw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpeesqdom.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gkckhunzq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ggpvnhryq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gbcyrtwyt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gnckxrvij.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gyrqrtmmj.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gehldfrlg.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/geieqzelb.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gwbniswak.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gcjqkpoqh.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gxyuwjtfx.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gcksdjtiy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gjhnxqsue.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/giizhvqce.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gsovoudvj.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gmcqhwuez.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/geobxqupw.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gnlpkfcxi.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gdytxuegj.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gtmgaqasn.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gqhdtctjr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gtvpvdmdt.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gsfcxpxru.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gmyesbqnn.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gaegzjjac.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/guujzmjdp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gmtqhkcdk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/ghhwrsspy.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/glswphkin.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/geyocdxow.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/ggsxhajfl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gwrylxvta.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/goxuaolpl.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gazzwyivc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gtcuqumvw.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gauswdrpj.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gdondqwld.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gkkedyqax.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gruvnwzsf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gbsckoudk.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/goompeefk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gepockotc.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gypcwhrwv.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gdmojzkum.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gzmnfbqsy.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gfxjblioq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gfteqrzau.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gjaiokmjq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gauobaejz.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/guwvpdbch.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gopyilirp.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gaipcslzb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/grknvekko.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gkbqrecea.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gmxqvnodq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gibgsyyjs.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gxnamwubu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gtjufkvta.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gqoxzkqvy.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gtozfyhcg.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gjpadfwgp.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/grefstlvw.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gjokvgtoh.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gsxmuajjk.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gomeeomxt.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gsunytlvg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gmehtvkrk.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gbujnrtbx.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gdmpcthps.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/ghghkhqre.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gceolcduf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/geckixpti.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gvivfnvfu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gxvevnzst.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpfsmvmyb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gdeckrgpd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/ghbtmiprx.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gvhftmcik.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/geobxbald.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gqgaxaflx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/goaxdjbgd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gimbfyjns.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gitjazfll.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gomvcuwbu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/grdhrpozl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gyjriihnj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gtxmzntlu.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gaveavfqn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gsveuluos.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gvmtznpan.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gurecsgyy.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxoxlvboj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/ggwtzydyk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gieowrfws.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/grvsvxzis.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwaybed.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/galqiiwhg.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gerpqwqby.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmrqpclcy.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/ghhgrngxz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/ghafblhzd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gkzobaikn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gdnopkdlr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/grdxiioeq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gltzcdonv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gyyuywbkl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gbbhxafut.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gqkirbkki.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gfkljinvb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gabinagkf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghjycxlkc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gmlvsqezy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gznndaorx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/glfodnvvc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gfnrvfakl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gfcynjuei.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gzalvdihe.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gubwfjgst.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gnzrjcojv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gwuixvbea.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/grftksjoq.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbecjdjhi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gnchxclkn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gdfdjtxmp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gvolayzlq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghtsdrwyn.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gotknuoeq.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gxyudcobo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gjckdupfl.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gihbozgwn.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/grefmbdgk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gdjggoifc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gpuosihht.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/ghtqmxfrx.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gehbkpgfj.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gltqcobwb.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gyomttqta.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gbjkyhakf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gzvrptplw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gttmcvjcz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gsmkitvji.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/givwfuaqs.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/glltotxho.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghkzrzuna.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gpxskxtvg.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gxcmsnkjh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gurcovcac.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/grlgqstpz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gdcjkqjwr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gqyvpanih.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gqlaosocj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gjfwrmbpb.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gqdtipqcd.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gdgiipjfl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gtawllhhc.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gsvoaskna.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gfutqqynw.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gicgktabr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gguqbzlpr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gjtwdanan.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gihkgymbe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxidydjvr.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gkedtznfr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gffihfrub.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/geatiousq.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gessknzxq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/ggmtxnziv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gjscqursp.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gzunaltrh.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gbrhookkq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gtuzmtjvu.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/grqfdgsyc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/ghdgklnlv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gfxtiodik.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/godchsgbn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gkrhhexig.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/ghjvrewyo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gbtwdjbuj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gbzcvlncm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gvioadftb.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gggzwvwco.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gpmhctxas.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gggsdyphg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/geeupazma.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/guerdaada.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/ghoxsmqoh.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gamszklsq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gtnclqmub.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxbvwtoxp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbxavrtyv.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gvaekfdzt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grpqvbydm.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gpmtidtch.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/ghhdmsurt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gpodqmpzo.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gtxltruzm.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gjnfxmnhm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gappjlymi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gvecyluyu.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gnpaiehsl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gdvjwigch.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gbpqxqnht.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/ghhhmkhgp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gznchzbft.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/ghyivamxe.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gllpscvqg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gtcexcwmx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gebswlflv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gajvxcolt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gqhthmspf.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/ggorcwbyw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gboawehmd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gujntomcg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/ggmrabtbw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gxtbivvfv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gppsuoqxx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gksryiwpe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gspfwogiz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gfigrypxc.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gedyeohze.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gfbwfnikj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/grlmhydnq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gtdhfjkof.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gjbyesdhs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gxmudtajo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/grrwnalqg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gzgwhlmhl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gkgakhyfu.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gpnmtwtiv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gxpmnboop.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/guwdahgla.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gisqrjdgq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gezrudeiu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gbfdahovj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gmiuirzng.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gwttxtbwj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gpulrqwui.sHtML


<!-- 参考信息 -->