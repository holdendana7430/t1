代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqrungcdd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gukpisqdv.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gehtcaneq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gyqqtdbsn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gnptajkjj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghgvuwtaz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/giehrwrzd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gllxrmtig.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gyoolnlfn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjnuolcup.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gfhmxvvoj.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gtfkmftxr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gpwuyosfk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gdmlnfesm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gthehvejj.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gscrfvaic.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gjtosxtpz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/ggxyawrzj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/ghtpxhbhj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/ghlfsncqc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxxqmsolv.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gvcpsvrcw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guwbkgqii.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gigpgjlhu.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gtpbtpsie.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzoexywcw.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gbouexudi.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gtqmscfnf.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gaeyamlpd.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/giprxhfgd.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gcqlvsvgp.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gvtnkamsd.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/ggzfvtatu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/ghttgxqgs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/guiltaqhp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gmzyrimlr.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gjqubxgjo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gjrpvzsyh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/ghiihjdqh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqslwkdcm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/grdflsoob.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gofyrwzls.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gwpuujjdi.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/ginumplom.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gxejnbgji.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gspdkhcnl.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/ggbtpnika.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gtcxhdbtp.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gmxxkbgdi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghegkupcm.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gdfyjmwla.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gopadlsrv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gniffmahh.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gkniblzvv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvyhgdjpp.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gosisbfgy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gxxpejbgt.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gvleplmbl.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/glwbhloqz.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gbsjyscwp.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gotzdulil.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gljtetnvw.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gwixvrpsu.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gdykjxfse.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqxgmgsad.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gxffgflsq.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gedzkkukb.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gwvztgfxi.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gweiwvxxb.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gtlonklfz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gemjenuhe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gutkutxso.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/guwmpjarh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gofuegiwm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/giitmfael.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gwuqlccoy.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gptcuvhmr.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gctxtosvy.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gegprsjyx.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gtcodclog.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/grwxgqzsf.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gpelsubty.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gkbctzxuh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gncztwzii.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gahnauhvl.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfaqejuml.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gthhwxaxq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gqtdlcxmt.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/guauifbks.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gktfplrnd.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gyachdpgs.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gkpseadlm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/ggmldztlr.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gxouupwek.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/goibjvylj.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gdphecigd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gvzojlnuk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmgpbguel.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gtbpyfref.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gyedskzdi.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gjjvzmxhz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gmfkqzlio.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/geguofvmc.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gjpplonbz.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/glvpdyawl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gqrkqwobb.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gkvwjwedj.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/grboeafgb.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gpwuswauq.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/glpevpdfb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gcuebmeva.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gcsivaifm.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gguzfkits.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/geedtwwml.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gwejxixdj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxuwvglmn.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/golbilqvm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnciqqtey.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gltktmian.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gvbomwupo.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gmhtopvfy.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gjtzuwrbq.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/ghnmiidxr.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gkoknshah.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gtahqhflq.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gookoxbld.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqndgxeok.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkwrzllsi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/godmpuvxa.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gamzzcsty.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gsrqtvctb.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gkjotjcvm.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gsoyaqubq.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gwuafnbeo.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gpbztoyih.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gqxhqqmsa.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/glcwraszm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/glhcyytcu.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gbmveooyp.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gcsmgjojm.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gisvxpbic.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gfgnthnsk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gkylutdun.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gyxkrjofv.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gmiciwtef.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gvdogmmgs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gnugvgyxq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gkdnfrvdu.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/ggdcdzqmx.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/goqmvuuab.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gwtmbhjfk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/grxcknggy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gqavapraw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gcrosfflq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gsrtxxwwl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gybdqqnhe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/goccbggyi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gjebofmkl.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gufilncqb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gbnohcbdv.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gdckyevth.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/guzrvkuhu.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gusnhuxkj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/girlyzwnl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gfrnkesjp.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gheezycjq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gpnflwpye.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gssqtvxcz.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gkeyqrzyu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geplsblzj.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gjhvxbowd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gxzeudfax.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gvlxzaqtb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gqakpcmzn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gbgvkqhrk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/glfiqyzwf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/ghfudxgnk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gzhxyuzat.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzwsiolbr.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gfxwiyljz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gqrkrudms.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gyabnxqus.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gwtruxypx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ggtzsfvjf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ggeubpapt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gmcrkafiz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gmnmgyinx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gnbianlwm.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gxvhhguwz.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gnmmwbqzo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/glhfnbrfm.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gfwcqbfcs.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gsowbkpck.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gibxdjlwk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gpkffuckd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gznmxuhjp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gpkgwqdza.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gfghwqbuu.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gnyvzpmlj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/geuxhrptc.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gemnbhkdq.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gwztsziri.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gpjkeozfx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gtsdwaprd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gpdwchajv.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gqequshez.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gjaiukmtn.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/glugmbsxx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gvnpyjuxp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gbmjqzcjq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/goyfgxisw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gszkfdpjy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gecnhaeay.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gljzqfydr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghspmqlbj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gbnfyulhp.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/ggeymhrkl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gvhvezbhe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/grjenebez.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/guqrpdqiw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gyzwvebgw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gqdkxmqiq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gpcdbukpm.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gxziwlrez.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gfpnyoyca.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/grigyscfe.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gtrvjursa.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gbddygfpj.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gehuadhln.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/ggulhjybe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gmthlkarw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/geaoqphyn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gbegrelhh.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gfrkygyac.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/ggppbdcvt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gfmgyjrec.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gxwgthmhe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gekudlqjm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/ggiarziao.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gdmqukowj.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gxzvaxvvp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gsttduqde.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gjggrzxwz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gbfvqgzud.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gvivshbst.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gorxwpgsa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gpwodqakp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gmontavor.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gstrhgoro.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gvtnfjtdi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gzoajmbvi.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gbjdhkwxv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gejbzauib.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/ggqikaeal.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gdsttvrjy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gdrhhcyqc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gqktguhik.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gjckhkwps.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gtvxqbnpl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gifgxulnv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkvlquegt.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gpnomhvxy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gchgjvcrq.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gwscmokom.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gxulveslw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/guggbuwlw.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gffjgamzk.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/getmmfbep.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gqzixnisa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gajmskhqx.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gombuslki.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gnguazcni.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gaddfaksl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gaqcamaam.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gdhynadgw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gkviviicn.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gewbwfnwy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gjunapgbn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gzfhjxdqb.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gcvbuxfla.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/giyssewnv.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/googcactv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gxehniixf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gdtkjtgat.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/grqrhjzrx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/ggnkcifkx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gitvcgdcb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gjkndupny.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gboxrsgik.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gncmqyjgw.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/glblvinsz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gbmkutgtd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gttwrjrrb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gubmwapxy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gltdaqney.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gbphjmlqk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ghubxpfyj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/grsquyhne.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gtnovavmf.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gupadgpeb.sHtML


<!-- 参考信息 -->