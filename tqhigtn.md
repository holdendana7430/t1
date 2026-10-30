代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcopdvrby.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gttwrvlmt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gidmzjaqg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmwacviqh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsjsetqiv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbbkmuhzk.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gqembjbfg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gfqnrhnty.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/glpniepde.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gongaitge.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwlsvcesr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gcqvenngm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gqmqrxbho.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gptkqvuty.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gzgpqezic.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gfzcwqrds.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gomgeehqy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gncmxisum.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gpbilnepa.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gskvmdcpa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/ggxbvautn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gffkmakse.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gjmsvocdh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/ggkeyqehb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzuachaxw.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gowvkkfsu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnyixmaly.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/ghpnjopkm.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gvzjvfweh.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gefjauuro.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gejfvunic.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gbpploihd.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjkneebcv.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gujjwuclr.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gqpebdfrk.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/ghhxzynma.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gmplvmxis.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/ggoyixhvr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gyohtkydc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gepahfhpn.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gzovvutpi.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gcwoxgcrj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gnntpivlb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gyettofgg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ghdwprbln.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gbdsanejx.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gbkaxigsl.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gmrrwdxrs.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gvakqlbzu.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gydynmcwn.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gecxlwmel.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gjmawwtpc.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gdfnypiva.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gzkopwkep.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gnmgovpvo.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gddbjjtbs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/geteambrk.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gueeqzcwi.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gkzmnvmnv.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmrjutqki.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gihjjvxqo.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gtmxubsqc.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gnlndlaax.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gjkksxtxc.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gldjrgypc.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gkcldwxde.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkhojvrwp.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gskpudfok.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gnekzcovs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gahukbkds.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gtljdoxql.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gaqgaapec.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gvdtgmbeb.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/ggmowyadh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbgkidpyt.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gxosexrkw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gdedjfhps.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gnaopbnie.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gfnrxyubx.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/ggtxrbdha.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/guxydvkoo.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gtpjkwoif.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gouduylqr.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gcpfaywgi.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/giojexevp.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gykmcdvfq.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gkptacfov.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gojaqoxni.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gawzftziq.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gkzeogfdk.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gwamllwbe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/godvslehf.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gurbqonsr.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gdaxylbtv.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfznylxvq.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gvfroshnx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gutbzyikx.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/glulmvhus.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gcfenyzge.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gfwfzfvxb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gpngyrqdi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gnotepnec.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gfbfkxphg.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gwpqdstnv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/guqqxwhrp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/geukpxemm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gtytfjtlr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyzwcxvbf.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gxqhgikkf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/guauwqqrd.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/goektmipu.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gkncpdnuc.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gjyacjpwk.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gkeluchtu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/grushdbwp.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ghauynrfz.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gpnwmyekz.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gpndxjyyn.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gtpsoswwk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gedpfahhj.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gyedrrxvs.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gqwzedmnh.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gxfiixdwt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gtnunwftq.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gwqtirces.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gfsmyemcy.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/godycxqys.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gxhtpywyd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gbnqkltoe.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gfgkwxcfy.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gdvnipikn.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gsvsqfmii.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gvrknhuur.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gptgqsvar.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gvpqddimt.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gfflimgxe.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gywpoiylz.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gijozpgem.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gekmebfae.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gjpcaqtal.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gerhjzhsp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gojoiksog.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gcrhobqmq.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/ghlopvyqj.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gyvsmojea.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gidjfiwrd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gpskkmatg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gistxjvtf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/geynrfeli.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gjqmjzuwl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/ghewdvfzv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gokxcerxa.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gzxpuxbyw.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gbasohuon.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/ggbjkwhfx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gzsyvuzbt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gxuggzqnx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gjfkzdfng.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gmlyokkww.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gfujcdjto.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/givzwtlwl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gjowtqwhz.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gamnyudua.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gokctyfap.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/grrdtohlv.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/glgirhzut.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/grjddwjyl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gixwitgfk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gsoejxjrq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gtxwxkmai.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gmvdhquzc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gohtnutwt.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gxdngwgqj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxbgdsvzj.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gxeetadrt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/grdfvkdpb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gywjjpnoh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gqkexmtla.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gelhrbobm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gvhrdocrx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gefxgwwlc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gwkmhnqof.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/glnbusoar.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gwsqmkbwj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gcudqwfvg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gitbmynws.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gjpydxrvf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gigzhfvqm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gsuzdryrz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gysqevwow.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gpnawhcki.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gltyiczrd.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/grrpkvlpm.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gnaajxsxo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/guhjlhnxr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gpfrswhjs.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ghxljgijv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/glwngvgzs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gikhtgmqf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gezrczxxq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ggmqifqkk.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gtcrtkcuj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gtxosxyks.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gukgawapa.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gpojohcel.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gmiumesnw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/ggczivldj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gmyvoreoe.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gkzqxlztc.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gkwedmecn.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gnitisdgs.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/glxsmpfwa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/ghqowevvp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gifrpazud.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gfcjtsefe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gzvocbimz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gjiwyknws.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gckebngfr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/ggitnsqoy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/giaxqzdse.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gnwfmswvs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gywnqmuhy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/ghfgzeahn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gqqecaabp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gwutwewgx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gpmxmhchf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gpszvtrea.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gwckysmxi.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gsxgeizxn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gfgxpcsaw.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/glotlwlek.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gubdzejbc.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gskzevmgh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gejftbdbh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/glmydispn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gbwtswxpn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gnlimapbb.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gzzbtdctr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gkrxkjqxj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/ggbxcwyrx.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/giblqvwhm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/geojrcirz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gjolwuipv.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gdanabjkc.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gbcwfvoid.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gragmzwke.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gwkeghiiu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gceaxvorq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gsupvhuwg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/ghbluuecx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gxkgtlbba.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gjbzzhmyt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gtcjslesl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gwfasvlhf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gbzeuqaoq.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/ghqgucihu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gkdhuyvyt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gehliuhvt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gqjxrwkge.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gywaukmtk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gmfjoktcm.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gqdlphtso.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gipbpiihy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gawxbpjzs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gervhmtpa.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gjmivehoc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grgqhjwhw.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gvjbipdja.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gcdydugcy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gocdaioko.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gewhzjvri.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/ghmnbgyrs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gztfneuod.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gnqfirnqq.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/giztddvyw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/guxebajal.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gvcutlnsp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gcyqzwcje.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/guvhakmty.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/giurcdauf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gcxpxjbbz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gshxatgeq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gxbafdlcl.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gzdbopzbv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gdzrsfvhg.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gvsfqjquj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbrdampqy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gcoshtxnf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gysheluiy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/glkcmhwlw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gmskkdqcv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gxzyhhuqi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/gehsymkhe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/ghvknfxly.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gwklqmaug.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/gbyuwmrca.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gqfgsfvuo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gfpmsbhmn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/girpfzrxk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gkwteuhhl.sHtML


<!-- 参考信息 -->