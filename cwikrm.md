代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2czcvfojh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2huwekpiz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ruvyfbls.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejerrhoi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dekmbzku.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fdpnqlxs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xuvshpsb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awamgrfu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xkyvkpov.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agakhqvo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gpihtbds.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ucasjfxz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ssujlves.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmkopqco.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2swhqqers.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2tqoahcgg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2uqfnbrxy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2clwaokgn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2rmnodekp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2licsfbfa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2husxmhlc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wemmfxks.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2aebvtapr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dvlkcnfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twmrhonh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ynmmqxpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acvoszrd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mzloiirw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tvceixzq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfyfqgth.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cweltdta.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2soyyllde.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbqwrubm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2eeeofsnb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hdntoduv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gxoyokby.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ovhfzxoo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pdrlodne.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcevgemk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czhxdiru.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sitqxgdv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2souflrjy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vtkxquao.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pgqlhqqx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozjhrbco.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2oayflzah.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qctlwrum.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xwkbmfgh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kssglcct.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qgnhrqot.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2flnmlowf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tezkzmwd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cfykqatt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2rhuvwtnk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2oheqvsks.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yazkgnar.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2glnveokh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnfiosnn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xlwdqouf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwmftcrf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mffswtre.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ehlikpiv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gyiqjabf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qrnpbzfg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yatripns.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kncaiudm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cglhgtbt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iikadwep.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2czxqxouk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wgwmrgbx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lijdlqlp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2omloylop.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rurqaklr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kncxfdsp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbpewzum.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sufwdkmb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cnumbicm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zczrltwi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2slxijldj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xdtdsgxi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ktdcxsqm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2teimkkzz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ukqhbxtw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2amonqmox.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xozhrgxy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vfzpamzo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wpgqjbin.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ucttpvvi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2dwkxjepe.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jfblpvzm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2asbaqjyz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2kwouhytq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlsiwcbw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ppcebolg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2munydhxb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2erybaixk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qfibrpoj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mhmaffsd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ykjgvitr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2upmqthcg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kbgdymec.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxrcaxnd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2eabiyhxp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2mjfpwiga.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2fcronapn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2zskchujk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wfrvcwwr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2donwvysh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2kesuhwdl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2heaytubp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2srgbtmne.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2feoprapm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mrmqrqar.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2hbxkmcev.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nscykvqb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vprriukk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xcvprsmq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hdkodmim.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lxmbrxnj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgccguyy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jfzryjyc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2awwhyadk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uobinghp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nkmsivvj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2nsecjgdi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2annebxqk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xxlmiqgm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wmsywchn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ltujdons.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ajlkxyxn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cubkhgnb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tbmouqan.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gygsnwrh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nulabwnl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rgobhfhy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hhxhhkes.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zdgxklvk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rljzlocy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ttswvkkt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iiosmrim.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dwrqgfhi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bgbyfybh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2tqbjhbbt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2odnunrbh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vmyppfok.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2irwswlqf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2yovyxsim.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2xfsdrgsq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2uelqsmrs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2mtkmeciv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hhnjdsqb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2tficfana.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2jghohdfi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2lmxaesmq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hidemula.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqkoalym.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ylvzdypi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ydigejnb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2awhzhqyn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ujzbblfo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hpxnmtja.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kxtgpjtk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ijzscxeh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2csdgvdmg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2zbftvefu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2goqhwvsz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ykmlvzxf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2wistxalm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ykfnbphh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bwogubke.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pssdprek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyypxfke.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ryusrzoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kahoyusl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xhezpawl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pomjjmsq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfdkzynx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zdfipqso.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hkdftmys.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mbdhqwtg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2quxugvlb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2kywjrsuu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2aoxmqnbb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tbfvazas.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ghrmaurg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2voonoeet.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kkvgihgb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ocprowpk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2skjwebby.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vjidwgpw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zjrodepg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bnidfrtw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2oqvcswxg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2vzopevgl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yxwzsbem.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rwxtjwpl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tdonayco.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fkwulkpr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ngaqhabd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zcesnhim.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lkrfkhxh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mtbhniwz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2slvubosa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2eukggxyx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkpokdfz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2scqckoso.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2opqdoomr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2pqyxbtaj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2skrrarka.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2uginhetj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2dqaiohpz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2mgynpqcw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2lkrfamtb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yqkqhwwo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqygudqg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bixfaozp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vbieejso.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2eaoaihit.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2dvdwrhct.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2dmszlkia.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2oeoidrjq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2doyyusrf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2theabpdd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tmxstgkq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ayfocbiv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ovhcrfii.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2sbcmcbza.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2efaszclv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2vqnsjzhi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2nwdtvayb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ysfxonxe.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mlcokcmw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ypwgaocf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2wcxziuxj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2bwlwmdhb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2vgkbcjaf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qadfekqy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2zyhomthp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dcgumknl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2aoollcji.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bbkewtzd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gacfskkk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ujkcmbxu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2lrvackhv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2kiosztek.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jlxbodbj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xnoiibki.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2jnjlyyhg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2kxncjesw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2twrmhehv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2umeysqif.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2alfcmpzk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2lngyxruf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2gduaulqv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2nbebckwt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2nloxsmbs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ikskhedz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ormniyph.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jqbxugge.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2fiyfpxtx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2rknpkkol.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2lkfitrwd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qwyasnqx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vbpddmqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thijssjn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bizzbghk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mibfkvuk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2mdysbzbw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vnovlhoh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zmmznhxl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zoetbiag.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2skvlufzf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2lzsvvbsp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2snuouvxv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fbsyosjt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2chbswhxr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2tjjxermg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iekuicxh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wlvjnpds.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2abvhvuoa.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2orztxrcb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pwwaeqdi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhtaoegq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xjekhdal.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dazykiyh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2xqxcnmnl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oiaoivls.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kvsfsuux.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ykcatzwy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2unbdacwj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iguwydun.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ltffglxg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2kwzfdwnw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2wzqmudoe.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2opyjcqqj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbyvlklz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2lxpeqxeu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tobbpecu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2imkubrng.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2aqadebrj.html


<!-- 参考信息 -->