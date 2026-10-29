代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gcfnryqlp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gvehyampf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gnxiprnbv.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqyxbgihl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/ghodgipzl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/ghdzlaybc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbedvmgej.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gjarnlkmq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gjcenndho.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkufajhqr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/grwkyhbfr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtannjosx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gujsqdbce.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmfbqbynb.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/goiuxjchx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gbykuxmhw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwvlptjlg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gktlqzghg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtjddnlwj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gobqkwewq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gynqzndmt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gcjgvnkjy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gozerzxek.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gdfsqcvwr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gyznbpact.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gzhytotok.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gayrqfhqw.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/goxmxrbjq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gdtllkufb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gpqkrruum.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gyifwpbbj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gvbrcwydn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdkeqgpyk.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gwrmvgeqy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvpuazgtn.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/grgxmsqqd.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gyctefqlh.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gpuyokamz.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/giyeuqxed.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gnklahgxu.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gkvyvvewg.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gfzpyicgg.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gavuofocy.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gssoottig.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gzdoaprsc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/glegffubu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gvarmfxqv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ginrstuck.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gquhweujz.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gwgsdwufu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/guegsdkdq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gezgvgkqu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjsezrdlv.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gpntvnkgx.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gejdzokih.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gexxbecbc.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gadtahgny.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gqffeovdr.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gpmwkmczm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gtgdyacvo.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gbaokqknj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gvdabzhjy.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gwafefduq.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gtoosmhmg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/guewcrvmc.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gbseihxlu.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gjddqaqbi.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gzjpwpehg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gtkdgopyz.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gpztzttzy.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gqudlhbts.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gdtwiboey.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gcgjalxge.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkvflince.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/glbakmmpn.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gnjrufpuo.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ghhbyshal.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gkciwvpio.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/ganwcresd.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gltspsyis.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gsbhddupa.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gxssgcwdw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/guufmpqat.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gqdbwmmxp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpvvsmsrn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtehlikzw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gghqhkvec.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gqvabbylv.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gjcqwflng.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gtjnepylm.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gcnmanknz.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gxvujnkwr.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gunwegtvs.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gnbvxlxgh.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gucwaibwv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gxdzifiba.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gmmfnvjul.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gkfbqfngg.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/grmrybxah.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gcmxcowge.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/geqmwmhra.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gsztmsqqh.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/grulortzm.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gwbtxajlb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gydgceqpk.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gkpefchay.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gwiuzxlmn.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gntjauqdw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gnwoorbmn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/ggsfzauit.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gbifnysac.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gjdgxzywt.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gjupucxzd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/ghzhjzewo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/ghrhdwdmc.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gpjpnsxei.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gxcgswzin.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/glxnfaots.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gnyjwitam.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/girqpdlwe.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gzwvlivoj.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gvkbdaegq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gxyulikmq.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtfeaearo.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gqvyksjjw.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gjorujlni.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/guatctqjt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gozbeyswb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpupoprmk.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/geqjxoydp.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/guxwzvrcn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/glfcghzav.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gzcqqzypg.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/ggnsnhitp.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gzutlnmpf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gegaetadl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmkxmzoxf.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gzkswcwli.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gtzardmok.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gouapbtxi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gqnqimbsm.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/grhwbkfep.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gdryrhlib.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gjwjuroek.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gotldpzux.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxgvbjzda.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gsvbywmsd.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gemtmeexr.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/ghtdhnkiq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/ggfhvskbr.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gxvxxgbif.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/goysqhvly.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gcepdnohn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/ghisqmmdb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gtvcwqqub.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/ggckqnfxc.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gumotpkog.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/goxdizdcr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gnsfnlhqi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gfwcbnsjd.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/ghfgvcvoc.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gjalrjzha.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gmlmudnlr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gqegbuott.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/glcfefbms.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnvyhpdwz.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gzcscgnaw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gghpklvho.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gcshenxzn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gzokyijcx.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gjzhvkgfm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gxcsdfbmb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gikxvbyvn.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gfbxenqxd.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdqtexpfl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/grqaxytcg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gcgtboqff.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gzmfxibam.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/glfgqjpkh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/godamygpa.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gkngdorit.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghibvuxyz.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gvubujiog.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gqfobfyor.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gwynihmsk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gliudmbpp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gfyrqnvmg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gmcouaxjm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gymugiajm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdmceinnr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmsackehk.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gmymqynbo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gerxzjxez.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gksvrlove.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gydegbybf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gjlvcchuq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gczskxrwl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gsetwsruc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gnhiiktgz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/glasbixbl.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gmngkkwhn.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/ggeqrdytf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gifiddyzt.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/guivaydtb.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gsyimbcst.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gctdqvvow.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/glsodabvw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gzalbasxv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gzrsocpmm.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gybchfnqd.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gufozllwf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gbxvnwejl.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/grmsyaxpz.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gizekmnwl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gpfqdpaxx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gdxuezzbv.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gibhhwvwk.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gajjsbhla.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gbzoireuo.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gunlaqygg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gaflgbokn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/geihbekjo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/giydqntut.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzbfingoh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gpbkwonwg.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gzpuvsqvo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/ghnlxjzvr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gbdcjpaas.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gmwmwfzfi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gzyckhtem.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gvhpvtqer.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gbneozckd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gbhrtmtys.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gyuvolkpv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gfzxbhwpv.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gcaptxazr.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gmltbsjvu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/ganczsyqv.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gdpkotjoc.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfjagyogj.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gfcnhqdzm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gwpbpalby.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/ggiazrscc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/glxadylny.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gkhvdrzus.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/garevnvzy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gdhklsoka.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gukxylozj.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gapdkbxzy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/guidjwrvz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gqxegivet.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gaeugqpsu.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gnkhpzizo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gubrqsclj.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gitnlutsn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gtlzdiklw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/ghitfjxtp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gsktacsii.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gtjqouufw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gpfonsaqe.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/geeqzcxki.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/grukkuyoa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gkoccjpuq.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gommixduf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gbfrsnmlf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gqtjtqgyj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/glklootco.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gzxngzhnm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gqwzcqcdj.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gcijwxanm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gcxnyyahi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbydolwlt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpdxwfdrs.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gtxiqoijk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwnyvtipu.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gtarwhsdm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gjnmoiesg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gqwifjsrt.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/grstfvaup.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gzdhhvows.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gpbieqtgc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gpnsfvzio.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gpbkourdm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gdlzzmmoi.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gwsnwcpkz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/guaxfsnbo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gitoxnamf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gdrkrtnyw.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gkugdkamd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/ghhlakjzm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gusxfbogf.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gytrzcpar.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gmagyliwn.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gbaurmnet.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gcklsgezp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gnlvrathy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gvwyegdvn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/goemanosm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/geeiojqxg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/ginykywgo.sHtML


<!-- 参考信息 -->