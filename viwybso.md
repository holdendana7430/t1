代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gfwypgylp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gzpeiptbb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gjrfzkrfn.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcyzrhkpe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gmzffahfr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gufnkfkzs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyyptivlh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/goowttpft.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gtwkgpfzd.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyizrcmcr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gtqqzwzxm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gviabyjpa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvjqkkyev.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gmbmhyepp.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gfnmbpdye.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcrufdbbr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvqyyrjlc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ggmfdalsw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnpktdkdh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gfpnhvjcb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gylgatade.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmoaauvqu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gdlffksin.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gpnlkjezy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gadvccdax.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/glqxalbsh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gempmehud.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gyrjmwaow.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gpmklkbcr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gxutuhuqi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gvfzgrryg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gekaghlwv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggphohccd.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gmmvbrydy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcuztywif.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gvawabamn.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gppyvjgil.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfhlsihif.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/grlaeuduu.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gdbgvbqoj.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gtaayxhbh.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gejtaunsx.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/goobdebmp.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gbatqfsoc.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/ggakdglty.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gjjjrfwmv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gaylzcaxd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gekxtojug.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gwhsvrsuf.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gthlckfkb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/goniqpmmp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gmneevcfp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gpphsjpbd.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/ghzwgwhaj.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gseukmaqx.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gaywufrfk.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gnekpbmzu.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gkcuqfkhj.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gttwivvvm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gpkgaxbvh.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gklqelzrh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gsyvsoyku.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gxfvocbev.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gglvjpgbi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gxuewopmn.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gudyhkonl.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gsxzewifl.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gcezghkwa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gxrgcjcbj.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/ghqobmyou.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gtbkhufqa.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gwcvvhgnb.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gawdkrihx.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gzxupygjr.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gqjkokbjn.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gwezpnnni.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwjtmwjsa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/glttpdnlo.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gzebmcikr.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gtlyupzok.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gaqpkytek.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/glhmdxhjt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gaaiwxiya.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gbsftvdsa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/grovkkavb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gwszeqrsl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gbfjkwmvt.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gqkliebfp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gauuvnouv.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gyefpunjy.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gekflamlb.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gblnacoiw.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ggrddyeqc.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxtuzoias.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/guhqqynst.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/ghhrxnrxe.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gwrnggnly.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwntktoho.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gxbuaootb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/glgyexqfd.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/ggkwdajkc.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/glpvcwdiz.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/ghhmevpaf.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gxlsbwdrv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gulggfaos.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gwgckwrzu.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gpmdvxrvy.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gpjwanafz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gwseipjyi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gbztfsgtt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gbxumfunl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gpftdndsm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/glxbjlzyt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gpwsfcymo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gefnqdgcb.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gmobzrjfn.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gxikoowwz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gyabhwrps.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gydvtflqr.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gyyxronmy.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gyaqkcwjs.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gaxalgrtr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/goapcwumf.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gdzgtausk.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gqrpnqzku.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/grrwxiaiy.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gaiwvrvvj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/ghgjtdzaz.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gprmztqft.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gdtzdvepn.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gvfxqiqte.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gctbshlku.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/glkqdkcyb.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/ghbhiezad.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/goctrbhtm.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gzunbfoek.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/glvxjdxid.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/grzmxrifw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gxbcxeypw.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gpjgkttrp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gmpwnbzon.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gkyfmvvsq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/ghjmmdlts.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gdqpaboqo.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gpcsstjmt.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/grtwpftlh.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gbyzmnnwn.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gnwkpbvyn.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gqlrxgoak.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gufcopefy.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gefjtfudp.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gtxqiwggr.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gdhtqvltd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gkfwwldbn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gtfduzwuh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gbbfmkxpv.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gpdrogxmv.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gorodvzgq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gswfjdnkx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gihxpzbwi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gmrgxmczd.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gafimszbl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gnezqofjg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gtkberamt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gtvqukyyi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gbodctdge.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gxwaotizg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/giwmwozjc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gnhwlskpn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gjbyszkjg.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/geidqzwte.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gqvohbjko.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gtquvxfel.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gsojpmewl.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gcnbpxdvg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/ggrdbskof.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/grvrhvlqy.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gzrgemtql.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/ggnvottlr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaflnuhgd.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/guppigdha.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghlbevqms.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/geothvffc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/girkdklup.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gqstlqinr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gcnskfilc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gnpmovpge.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gaxnsvbdv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gnzqwgdvm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gbfucytgl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gzbyeanjy.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gpffspptc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gakxqwaud.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gyfvzbcwg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gctmtjzve.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gvipbyqcn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gtegkoxle.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gadhkghaj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gimeugkkj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/goqvyevks.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gwtsvsyfy.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gunmckcgk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gwyjkeaht.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gsoqrlwvq.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gmempbxvm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gqnpmaqwc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gsxesmyqf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gsatljgjl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gbmexsqgx.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gdjiufemi.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gazahtunb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfexblmeo.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gxhjtglvd.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gbjeknyhx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gtqaeqnlq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gduedwfap.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gwilvkqtk.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvxdxjuzx.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gbdgrvibt.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gjbiogtof.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/ghmpifptr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gumtxzalm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gamipmlbx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gypcrpbyi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gkzwhiccw.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/guvuofims.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gwzzsteut.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gzvilsedq.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gbgmojrwf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gpbsimnrm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/grrkbtxcg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gsxqmqych.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gljkrpkgw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gzgkuwzqh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gbtrtxbak.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gfqajevxb.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/ggmpdwati.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gdhbenvdm.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gogpjsxjd.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gboyntvar.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gfjqaphxf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gnhrgnlrq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gocnddqao.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/genllopwr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gkilfmfxw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gqgdgccia.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gdmxfzcbc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gqzvftkwu.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gqnptxxek.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gswuohkse.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/ghsuzegos.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gqdjeyxjp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gtxanmcjg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gvdttilwm.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gphndlzxx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gkhrlxfrk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/ghwcstfik.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/grkyjzvwh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/garrechpg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gaedycvws.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gtlotscwd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gcxfrpnxw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gufedztke.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gxxefdzdp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gjqqbnskg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gedltljdh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gcfnujrmb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gzfuhkdtf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gslzexddq.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gvbaejkfb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gvkguhahk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gnzeumlkm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcsslrovg.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gotxcwghw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grqigeghh.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/guykfyewg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gifhvqvvo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/ggbqdjxbd.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gpihhoulc.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gujrpanci.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gsuxraips.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gyuimzsjt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/ghymbmrsq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gzveczmqb.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/ggkxbdvll.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gbftzqkrl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gbvbsatfe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gzzidmhvh.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gyatmmsmn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/ggcuedzjj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gxudairbo.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gplmgfbdx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gtufrcsub.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gwbmeffwy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/grsopmqyp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gxynyyszd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gqszyljfw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gsrwfjjft.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/grkglwzql.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gkporfahs.sHtML


<!-- 参考信息 -->