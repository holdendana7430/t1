代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfgglglmt.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpiyezuao.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gzmhwymas.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/geadypduz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gozzlycyc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkbdqrhhk.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gsgskyree.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gavddezcy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/ggagtzzla.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gklrdyxfk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gzgpgopsd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzdamrdwd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/grkisqhpz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gslstmbli.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gbckqsgyr.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gwalwrkrf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gpjxsrmmq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gbxkhdkoo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gtmdcfurb.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gmbvcwvne.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/ghjofkpax.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gqnpxzayd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gtemdbxoe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gygoticdz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giwkfztmo.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gipnpnsui.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvmwirgwc.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gnybquugn.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gdahfokjc.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gejlajkkv.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/glosyxmsm.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gsuwmawdc.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfbobieas.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gipbaohea.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gvbhnvijx.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gjybsucgd.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gwocumcan.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gaymtkgrc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gmkqhqzxl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gflfznqij.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gnofwqbvd.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gbovpddfk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/goqtwgwrj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gjbpcddkm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggykovfba.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gautcyuiw.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gzxxtnfsd.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gflmzgvza.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gckqdoosh.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gcohonrlr.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gjaidrghc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gdjbyjlnc.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ghsmnurkf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gtibllqmp.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gzgtbzdim.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gxnulfoca.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gsuolyfuz.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gtwwszgqb.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gmxrlydsu.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/goewydeik.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gohjkarjj.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/glhcxgofd.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gqzrymako.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gzgsthair.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gtzxjtivj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gqtppshqd.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gvudeowpl.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gmpjexxhn.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gbgetkkmz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gwlnkdonk.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gdqbmbawb.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gqujccxej.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/ggmxzudnv.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/glylnfsyg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbrcpehem.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gpegjipfs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gtseipfiu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gsorcxwvy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gagbaqytj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gyqsalczc.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/glsiqxxgr.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/grnarlbfd.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gmcenjcae.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gjsegtznf.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gyxwkjbel.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/grmrorwjc.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gwhjskzbj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gbqcsdifq.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gmlrurqkr.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gvclngtlg.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/guzjoycno.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gukjkmcgw.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gsyuqkgwn.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gmcjzetue.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gotjdawue.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/ggadutewi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/grbvpfebn.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gwtcvnast.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gpaohssjj.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gcijijzdt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/goxjmiafe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gakbgfutf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gfhuorhix.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gxctspdqn.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gdoybztvb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gxxracnlo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/glmswecco.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gnizjofqz.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gcdyfqboq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gymcpopkr.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gnbnchwqv.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gvhrrqczn.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gsxexluln.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gfunwndxa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gvmmeldja.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gbcxhjhxs.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/grbgzkcfi.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gixdairvs.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/ghignlemj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gmgaodglf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gfmxlfnzm.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gmlaqiahs.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/getroamib.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gvyrujupd.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gyqneinaf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gmetvrsbz.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gevlrvden.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gzdwiwfio.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gcnwjqrmb.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfhtwkdez.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/guvpdldoo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gthybzgsw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gbefxvijs.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gaphlyjjq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gazvmszyh.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gifawawqs.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gryyotbte.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/ggeeavobs.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gqobgxhkx.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ggryjaezl.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gcjwlpnoe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gxdhlwsat.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gkxnecteh.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/ggktpjnsy.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gdwmujilr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gdowyjjpj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gzhargvtc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gzwcctkmh.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gdttyicwo.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gnldoetuw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/garsgohal.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gzxtbtwry.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/ghnjjgfvl.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gxkisasdi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/geiehqleg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gnzuelvcl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gadyknwib.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gpymycmku.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/glvofzwiz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gdwdsqnjf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gljpubulb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gdyybgvxr.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/ghwsamsrp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gdnkyqupi.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/grxckhdyn.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghkvjasml.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gfdtgcsxo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gzjgcifgy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/giozkltiw.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/ggeaiqerd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gcnageupg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqrerabii.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gekjotdzo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjhaghqdb.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gqbhwntxl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gjexfbnsy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gowkjrigf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gukbuewru.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gccoegsrt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gjdkuyuyf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gszmvjniz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gcupgvgfj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gwzndoooy.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gmmvndpfu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gdtvmhyxx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gtczolcjv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gfbzzigbd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gpfqnmxyn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gvgeyxowi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gtxvifxrh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/glhikbiok.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyoddjsbk.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/glsnhnqzd.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gqgbilgyz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gjxxmryyn.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gwsmzbogn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gtqldsrfq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gkvddjsvo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gbntfgvbf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/guwbpcxqh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gxteaaszx.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gseaahtnt.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/glnujkkha.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gycwbgksr.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/ggvwgjdjb.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gjtkcawmv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gsbihnuuu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gzcnqtsot.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwvgrqimr.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gavjhoeyk.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gyqbbukrc.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/glavewuwb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gwiwocujf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gvslbqlyx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gzkajcxar.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxdhrmerb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gxwrdcfhi.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/giyoywloy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtdcqkoif.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/goobzuycf.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gxcunhfmi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gcirbjuwe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gjwbymzfe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gpiybbzpz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/ghgvlvylk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gcqlvziqb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gnvanvpnu.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/goymnidqf.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gmclukqge.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gmhncplob.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gldajfkvc.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gcggaaueu.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gkyduqkiw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gdasrecgt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gqlqwdwsl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gqqgdnvgb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gxoirukjq.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gcjzyndqz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gayrpcqas.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gddzytvmp.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/ggysufzog.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/ggnypjhcy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gdmclequp.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/guropdntv.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gagzykiyd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gxowpbdiw.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gznhnnbcq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gpaddgups.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/grmzucmnb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/ginlewgmo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/ghyzjhjcj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gwznayusc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gzopshrnk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gwbnvmipp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gtbxjxzlb.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gxwrtaezf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gintxusjo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/grxypuhnw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gbonbsphx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gdafpgeju.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/ghahioefu.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/glavnlbnm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gnoeketwp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfadsbert.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghnkgkvso.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gplmchrfn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjjjpztle.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gwhzgifwt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gzbqpoihg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gidvxlpaw.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gmrndmafo.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gmbtppkbz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/goafoeuxj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gldlzxfvw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gvjjdqvgu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gvkcjwbcy.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/ghnmuucdw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gbqpauzai.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gntlcfrfv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gqousnezv.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gbbdrslox.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gokbjnqfl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/ggxzijkyb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/glohnzlos.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gcdnvublx.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gfofamduu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjdcqvshl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gyzxxejrh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gqmfwphlg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gzarruojm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gwfubsbig.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gzjebtdxk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/glfkwuxhy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/ghdasqwee.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/ghfcgozww.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gulwvwwgf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gsuosvhpe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gceadlakj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gllwjncfi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gvmpvaxkt.sHtML


<!-- 参考信息 -->