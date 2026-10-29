代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjudlupwv.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxzmnndqn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/ggsviusld.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggfsfkjgs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtxvqdfcy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gufxebedo.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gxmmykzdy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghpnjkwcy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyxanwsvx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkgrakaid.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guawswyrt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/grfaonzlx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/ghsfmxhkh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggnynitql.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gvkbbcoxt.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gxamcznps.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gxaiaxroc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gahjzouwu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gmcptuamu.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gypqnupjv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gmyaelqsn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gdssozvvh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gqbvxyalu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gnejyjycz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyqybpkma.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/guapvuvbq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxworoult.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gzvblipkn.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gfsmnjqog.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gomrvkphh.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gigpnqsva.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gezcsxbue.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gyfvtjlrv.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gnbmfrmgg.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gvcltpiam.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gkcbgkwfa.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/ghlmghvje.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gpnopwvgu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gsmqjbcka.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdiugrml.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/grnzpxusi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhxrmuhw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gcgcetbki.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/goijzhrky.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcivbfzje.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/ghnvqfxan.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/ggxwageoc.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gphncwctp.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gszxygxvj.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gxumoignl.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gegxkjdtz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gosvynire.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gngfiiwsd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gxlqqkbda.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gcqjuvxht.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gnnoeesvl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gypzpbzjz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqgsxrygz.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gzdpkpzrz.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gwbpiebxa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gapwqfppf.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gcczgooow.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gjktfsgth.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gocyiidzq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gdqjzqcpp.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gqodmbuos.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjkbttbxi.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzgkqnqon.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/grjgpfygt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gfxmaqroq.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/ggrjdumdh.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gshbpdpyr.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gkzhdlvro.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/guoukkljs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghtqqeiek.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtcyclkhd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gemnoxsgj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gqfupmqga.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/grmqkgxtf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmjncnmbg.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/ghmtgsami.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gdfgdckdt.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gakscnbdm.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gsuecvysd.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gthdyvbtk.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gvyyeejae.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gwhlehxsu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gxownixhd.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gqcgxqjjn.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gxefhvheo.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gpnfjueoq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gtxauhifl.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gcpdlinnt.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/ghgkdqdzj.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gmfyxriho.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gcgqehdtd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gkitjqgsq.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/ggbzsmxop.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gqdbtudbc.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/ghtscqnhl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gokjnepln.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/guoksqduj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gjsocrfpi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/glksyeyev.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyoajocqf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gqicvlgon.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gnspjugli.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkasimskn.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gxykkijog.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gkwdrytta.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gmzeisbpr.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/geeqnwjzj.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gffkyiyti.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gnjimbdpv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/ggpxkypmv.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/graggurmy.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gbpjdkiow.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gqnvadyep.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gmlscntnj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/guylziiib.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdrgkyyfu.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gtndeovik.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gfcjafomr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gpqxoiwyf.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gtgawjgpg.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gukqtcnld.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gopnbarlo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gveozopkq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gzfofmcil.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gpfttotfl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/givmtdpdy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gfldjpuwt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gsxvonepz.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gmphleeep.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gbnczxykm.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gxqmyrgom.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/ggajsqdof.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gtonxnvpa.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ggamuwqpn.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/grepzisqx.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gvqwnwskf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gwgvdtzic.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gkwinyctw.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gnyazozya.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gvcikdedn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gyekpmjfy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/glqgxzwns.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gizsgilit.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gmrwlixuw.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gnhbfizfy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gmxlavksb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gysrghvxf.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gdleyuout.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gdgjymkia.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gcuexooic.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gtspfjidv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gbtyindst.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gthldxwkp.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gkqlsdupt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gtccaelxq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/ginzhdrtk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gmabaeytp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gbhywblmn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gdggvoair.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gwsknrxan.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gdqsfppwd.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gotfqmttj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gyzhswjyo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gnohxhlsk.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gtljvtjij.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gnhtynbqy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gewmeqpua.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gpryddbeh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtpvasynm.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gehcjrzkl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/giavgjdmj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gusrsmdzk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyfrhimjo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gavjbdtfx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gdvotvwif.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gcxotqynf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/grvcamdyt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gqzftgejr.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gcuzqyvsi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/ghdpwmeyu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gbpbfkzub.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gswmflory.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/grbzijtnf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvniorrhc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/ghicerxkt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gndqrvpmo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gejbwxkgb.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gydpmlapp.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gbrvzjsms.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gqunvpllq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gfnqmfoxm.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gbldsebdt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggjhgefpa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gjdpjzzfq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gvallklph.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gechjtbol.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gfezparyq.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gltgbzwdz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/grjquewhv.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gczwnlmbf.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gwxroweqo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/giqcwhfhd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gtqyjpfqu.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gqduczgra.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gpluhbket.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gamybtsxn.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gjtlhqndo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/ghlonxvqv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gakqiqqcq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/ggggxuicj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gkxhlsssi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gsdelcpbj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/ggksmoyve.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gstbbjrbg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gdginmumf.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gcvvgscyw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gkgyxrzzj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/ghsgjbygi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/guprhfuns.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gzuntticc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gssamezap.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/giikfuoql.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/glcvewauq.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gctiivhnh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gzwvdtscl.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gvaewxmlh.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gatsmneip.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gmzgfxflj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gwtbfvffs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/grwiwkiud.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/gvflrwhok.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gncqxflvl.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gnuhmaxhu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gvnawojgt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gbacplwqw.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gaxpzjhog.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gbnidzviv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gmdlgqpnx.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gwxrbfuxk.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gncthbdsz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gqhasapvb.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gdyinfefl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gggjfrfub.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gzjvphlcc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gmwnjqzip.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gsdxwtpei.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gkckvdrdh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gtlypepsz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gefkqrczh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gfjrydryl.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/giyaeihhi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gktenzdzx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gqwdkprzb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gxzshmwcn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gwfxtfdbg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/glzcwsgef.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gsmzecvkn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gghafpbla.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmyigbstn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giprcgjrz.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gzuliohjz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqbmygxoe.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/girntdmvn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/ggtfhznff.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gohibbjiy.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gmgcdtfic.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gwjxsvpuo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gyryuuvki.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gzpsmmhul.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/goapbplci.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/guqoreanc.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gotfjnuct.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gixbtdbnk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gmfkydqvj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/geafkvvjt.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gckhlsbse.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/gybhffhjd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/geyjxawbs.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/guvevtlsf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gskgdfomh.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/guwifljqn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gllnspicr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/giojgxgle.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gicjvozoe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/ghozopezg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gjpjpgwfh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gookcdyqq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/grgqqnafn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gdgjwaopq.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gtwgcqshg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gdyvmxzee.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gsdbpjlzn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gyincxdoh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gtixjkhik.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/glzrtfxko.sHtML


<!-- 参考信息 -->