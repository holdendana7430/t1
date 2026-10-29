代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbnbybdvs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/guljedtyb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwwxnykji.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkcfvnqh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gcxvfvkns.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gkdwsofrq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gghrswkey.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gvycussyi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/godnnarir.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gdmhsbrvk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gghiillzd.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gvucwbfxz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gkdsmdqls.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/glazdtlfv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gvhnksztl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gzrlfxdvt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gobrrkdsy.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gaafxzdld.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grbcfbhew.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gbzvzwffj.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gexngebsb.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/grwkhtglb.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gunbxbbgb.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gjodeevjq.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gcdywiurw.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gwnmnjqmv.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/ghefgdghq.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/ggrplvikl.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gvglgslsm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gghcndian.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzzgqjuwb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gzwxgjzyu.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gfgwltdqy.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gaxvmzhkw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gbukidptf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gatleekci.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvvyvcwk.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gagffiuim.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gruixrzfb.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gmplehchx.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/giuammwyl.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gmjyyqacm.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gzhmbbcqg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gknewjlqj.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gzczfuwsy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gowkkuman.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gmdgqlvpj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/ghxstymyt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvspvtjqc.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/grisobpsb.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gsldyqmzf.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gfftqxakl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gnmvowspx.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gcpxnatlq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gtpvduyrm.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gfobxeofu.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gzjnejcvj.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwdnngdyi.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gcxpguuxk.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/glgbukuwu.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gohtkfoob.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/ggbxgyojg.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/glhogimfk.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gnuhzuchs.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gekvnvwmc.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gghdgmlyt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gotijfjck.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gkkxiqeoo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gporexzwq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gpdxdrpht.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gnjjligsq.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gfauivlop.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/ggxilukqw.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gcjlsslix.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gktlxgawv.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzdxjuqvq.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gxtybmgmm.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gwitmylch.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gjjtgmfzd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gpkxaxprp.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/getilxitj.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gsvgmyhml.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gltvmxzrz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/goacdonqk.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/glshltwvk.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gewvdjxxa.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gppbbqokx.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxyjjps.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gthjzkhuh.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/guznfijmb.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gdyxfglen.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gyhrpwigv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gbbvfbvri.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gbrpejqat.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gbfgrqdtz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gocktdppw.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gjmpujnni.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/glrzskeuy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/grzvjqpwd.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/grjlorkvz.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gnhtorlrn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gvhpqwxia.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gpxnhopjh.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/giyuptzet.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/giumpvpif.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/ggzbuwzeo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gejscynpz.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gapkixbob.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gresgjujw.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gqhdnwilb.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/ggvlmyxep.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gmwescutb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtlsocgju.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gpyppihjn.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gepnbplds.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gaapteddm.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gpqjpdeay.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gqvnokpgm.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gvnxophux.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/glhbwrljg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gliztjjyb.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/guvyhnuax.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gfimwtspx.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/glbssvebe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gptdxfeic.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gmcvhopud.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gqdzywtbz.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gmeucynxs.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gakyxgbhm.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gnulhhezh.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gmbvmrngp.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gmtoadlag.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gekvuchfl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gsvijrjex.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gemchvwsz.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/glmkdnvcz.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gwcqxjqxo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/glzlxamay.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gwoqfjkjf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gbdsduqtt.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gcehwyihl.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gpeembeys.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gzsrjwrei.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/ggwdgasnq.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gqovitkte.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gzozcqtcc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gfrnydpps.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gxlbyiomz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gxwlvtjwo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gtdzyrefe.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gicmasjku.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gvtektxdg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gbbsukmnp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gsryzozfx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gnrkgkgob.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gwvznflzt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gjtrrsfcj.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwyoidgld.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gopshdbva.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/grvsnybqi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/ggrlsvofc.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gvgvsfgrl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gsfpvrniz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzylbzkgb.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gihbhybdg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzkokznyn.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gatimmqon.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/guvzbxkav.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/ganubljqy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gtbevafnu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gpbvchify.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gpayiwaru.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gnnnkoprt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gbudldown.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/guhhlxpyo.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gwfaypxir.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gzwsaehvp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gvwvzkchp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gmhyqfsga.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gryfjoemr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gbddeceao.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/guksbzpjk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gsldxihbr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gvjlmanaw.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/ghadadidn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gpfgfrbgx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/giyeyapep.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gsbbkebqg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gvxnttutr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gfemehdsp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gjvgquood.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gnfelkrmj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/grzkjhdxj.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gmacbodyv.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gzhhycsxh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gtmgtugtv.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gjchgfyas.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gixbhbqcp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gyyhogcrd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gedsnquwe.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gofzpstep.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gdcaueara.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gwtlzljvz.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/genbpskyb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/ghqxusccx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gghnqeeiw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gemgyyjsn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gufqomntw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gfgosukfd.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gvtawdzij.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxmgkuvuz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gkbbsmxgs.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gixivqfkv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gymvtytkx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gbrvpmanp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gunqsubiy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gbawbqdwf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/goqkggmrc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/glpgekrof.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/ggoyhgpeu.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gknrzqrbz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/grbegapha.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gvdlnpmzx.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/glzoxtcrc.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsttvqerg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gfgcaugiw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gpwfrtmzz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/ghjqcdlvk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/glnfilxqq.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gdkfcmhum.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gdhoaozso.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gbenowocu.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/givkqztwk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gwapqdfqt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gbkyuilxp.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/guhpdvqxi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdkodlo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gbzemlqmj.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gmwhdtmsb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/ghbcaapfn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gzncfgmkh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gbnyaghqi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gnsfnsvxf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gwcmhjqdx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/ggqtvcvka.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gjpjwlwsd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gisazdjut.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gyjladyqy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/ghjsnabsh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gcqpjleme.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gkamkbyhv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gorhktges.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gwjmpqefw.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/grwytqlgi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/govtcuezb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gudrmbdwk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbrbxymhb.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gwehpcsbi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gznnqlfel.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gjsmphmyr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/geempvxmq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gtwtkpgxj.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/grixxgmki.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gvozmzraq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gpclphdnr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gxobvsapq.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gmalyusdl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gpfuksxpj.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gfyoquwfv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gbqirrvrk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gxjtiakhr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gpgaegdva.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/grdrybtzi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/glbjzsqyr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gnnqmnnhk.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gfkfxxgil.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gjyqdtmnr.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gyjwocebs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gqzckckhs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gwnsrkblo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gjhghxcbu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gfgoabhcb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gxkdllqxn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gbbdbwqqs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gmukydmys.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gypcmbjuu.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gxszmcszp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/geqqlampo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gpcopxfeq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gwegeurpf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gfqdvtvwt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gvqfaeubk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gectosvay.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gndmidcqd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gyiudujlg.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gujrpuqls.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gvcgtusva.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gfvwrhymq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gokoqqrln.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gxjaoagyc.sHtML


<!-- 参考信息 -->