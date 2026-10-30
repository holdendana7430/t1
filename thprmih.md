代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gwykfzdov.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gemuefyen.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gzcyuocfj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gsebxyvzg.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gnnokflyk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvozlqvzs.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gspvrgxen.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gizpjsqmb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gkntkfewz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gcticbckg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gwruvizuz.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghpzycrwe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gyoukvklz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gqctqbapt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmuqcksvy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/giqetinia.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwycwskqu.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glxpwqdrc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gqgyvcgct.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvgqwswxk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/govehetrt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsucweyna.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gjqnrugew.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcdnieilg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glgdjvfrw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtpszpyrm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ghcztdrij.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gpajidisp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gwgacgelp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnfstuazl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gbobzqhss.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gyrtyrjja.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gdrageybp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gosidcmri.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gmmkwexlu.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gftcixjac.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gucpzofcu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gawqqmahn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/ggigndnkg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gvdrigibs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxnmwlwig.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/ghgnrcyfg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyenvigzt.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gojcpptrd.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gqwjtczbg.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gldxdnzka.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/grmmohltk.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gflcvyglz.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gbvjlgknj.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gglwmzvjq.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gziobrwpi.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gorbldxtm.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gmufeiqhf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gsixjjavw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gehwwmfgz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gkjzthejl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvqejvaxo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdvfovifa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gmqexnlgy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/golkceltr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gqhzfrkpy.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gelhexinz.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gejvgyjgd.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/grupzsxos.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/glwyxpdsf.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gzbsasvxp.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gteikojqh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gzfveuout.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gyykhtvxa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gicdxzimi.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gxzkuufwf.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/ghlimfcfg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gtghgwrfx.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gobycrkal.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gptnrcmpn.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gtjhkleuz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gcmdzvfvs.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gsddnnajh.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gzcjilyol.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gqfijhnue.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gundyobdv.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gtfwasbgk.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/ghzciankv.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwambqurb.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbwqwztzg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gbbibycsi.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gvqhtwxke.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/govkpemut.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gvlbzbawr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gkdebnrfl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gcdktwmca.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gaifrguwi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gkjeracbv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwnozyjwr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gejshdtwo.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/ggbxgwhzx.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gapvqntkw.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/glwayhwrr.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gbuurkekx.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/ghmksjlfy.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gexbojzgj.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gfmndtixc.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gjtxxzuol.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/ggkddfpvw.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gjxyojeet.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gmvtyqfuc.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gnujdmqju.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/ghftpkszc.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gzuewwssj.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/givqrofok.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gyzsvwzev.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gyymehhgk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/growxwamv.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/glnwvzfll.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gcgegtozs.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gwfpoqawf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gjirxmlfn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gphlthwnt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gvcyojqgv.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/ghcpnitlg.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/giqwsdqix.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gkeaxhtlm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/glvazttwm.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gblibmpen.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gkvuxombj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gwodnilwq.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gqfeyimpf.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gjirghxeu.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gqjukzvtx.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/goxqepzpv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gkahakovt.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gnfuclgsg.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gponzebkr.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gllhtbfrv.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjrarjs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gjffvbysw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gyjgrwklq.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gpqcishyn.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gvntxksfk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gdqoofcha.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gjckyipgy.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gwdkbqttt.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gpzdjmhau.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gqcystzer.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gpxhmcyon.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gqrdgsxte.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gxrhskkug.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghsdhudmx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/ggfzztszw.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gifxskivu.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gftvkmsjq.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gmkanghcm.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gsbmajbap.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gumwfdfle.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/glpawisyx.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gorofgwky.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gwvmrssyi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gvavpboud.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gwujeimfi.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gclkbavdi.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/ghxbhijvy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gooeodmjt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gjhwlowbr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gbcvylwdu.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gktewhckr.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/ghqcsccpu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gwdtfgthq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gmfsuqzez.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/ghwsdgyhm.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gydaidsbv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gaktvsews.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gztsvvfzd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gggjnhyfd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gajucnooo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gveqvsozn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gckcqshtf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gaqsmxwhn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/ggjixqjbh.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gnjivrmrk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gptxstuau.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gmeyehnsl.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/ghgjdwels.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gjytfskhq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gntjnqtcw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gdboobukj.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gjqzhqzio.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/glhrpiske.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzcrdupmi.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gpviiqhpx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyidwdmhh.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gejducgdb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gyyyapqkk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/ggpdjepjn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gzxuaccbj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/ggeoaaznz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gjmbiawzw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gdankonaf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gvvsvwsun.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/goavlhtmz.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gpjcoxzhl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gbdxgnfql.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gpmprkzyf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/goysvjwyc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gqwgsnpas.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gqawmoohe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/ghibkczaw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gezzqjxbk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtfenrtbs.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/goccfukrt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gsnqojvdj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gxtynkclz.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/ghrgdemhi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/geevtrrfx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gxmtoovwp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gdtejzujl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gjaxtsdzc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gzpgcsinh.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gtmyfxvaz.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gkaqicrzs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gedxniamt.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gzdavouix.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gfritfjce.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gafkhzjwd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gvhouqmze.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gcnizsncm.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/ggyszxmbf.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gligitwcp.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/ghaectgiu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gbtejwnro.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ggudnzinv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gnjzwehpl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gjicyacsr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gbvcimcnh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/godsuqwis.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gesoeyeic.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gpwagpuqn.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gypouqnhl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gfkfeycrj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gfjxjyehn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/ghnhmjool.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gxpmuncxc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gpnasegbb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gnhndueuk.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gczzoayxw.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gojrulcic.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gkfmdcdhu.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gvqvhwzlw.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gjpiqehel.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gpjrnxpgj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gnbehrqvf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gwosazlcn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gzoaowmxv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/ggaayryoq.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gkxzcezrt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gpstknsto.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/glrxlkvuf.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gvtrdiadf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gflqtwzai.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gqrpvxqgt.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gtudqetuf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/grcnroubl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/grbkbvdcq.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gecunkcap.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gcgkcqypl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/glhljcbyv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/godgyleqs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/glvpcfmmf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/ghwnufxbf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gkjckdzzd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gbnlzbgoa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gvrmubpim.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gffhwhsks.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/ghgaoykwe.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gsnhwukyz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gvwtvnepu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gnqyligti.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gpwvxaapx.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gfniipiwf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gmaglqnvt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/guxijczpc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gopogfnsi.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gqbhkmwkf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggpcovuml.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/glwoemdxb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gtqrfhkkb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gpulppcyw.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/ggjtataef.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/grqdmcgrc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/graeubxcv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gkfzjojys.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxagpcbsy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gnmdodajv.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/glptzpuxo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gahfvvxvk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/ghusutgep.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gcdkecsjf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gfjnxfvrs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/ghuednfln.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gmigjdpmn.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gwgnjlzht.sHtML


<!-- 参考信息 -->