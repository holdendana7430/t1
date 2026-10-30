代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gwzetqlvb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gvbdiumlx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gyihqqbum.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gsepjkhit.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gwfwqbrzl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gefgdfynj.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gqcfzyrzq.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/glmzsoeye.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/glismlwes.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gmzajsvhq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gxelzyioy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/garhubfxn.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gvdnkkcea.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gamtgroxd.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfmpjzgan.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gzndtapqb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gvkdwdgxo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gsgjctwuj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gaznufeed.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwzzriwdx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gdotgkqyh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gkabsuqbt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gslsleyam.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gldtkqjzb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gebgvztkc.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/glknlmyrr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gwartathv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsytfipif.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbrfnhevs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gywupooer.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gjputzwie.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gywyaknyp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gfuoyoyty.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gfhnkflgn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gtgbuqpiy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gpkbddcbk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gjbtjaugm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gecoeaswk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gpojmqfjp.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/ggrfvhknp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gatjwwbtx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gdmgxrfjq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gqtsbpmnn.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/grgidkfxo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gpbuczaih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gkcclhgnk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gjaaswcmn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gmxgtnfrx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gamvuzitu.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gxxsufgws.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmjeseder.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gbiudwqqj.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gyggqdyhi.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gfqfxgcmq.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/grbztpmlf.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gyntqjnue.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gvriikkeq.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gqeapulbg.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gjijxuyoo.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gdaefsuqc.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gvrdvfdla.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gtufhkrmq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gqohubesw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqtdzehm.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gpqrgjitf.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gwzmwbepo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gjqrhplox.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gqggnkbxy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gmppdioei.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/ggajomtxy.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gcwuqudsm.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gspeixhwg.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gfzzzrnjp.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gmvcbrzxc.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gamehsmbi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gezhriyww.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/ggztjdktj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gjraomxll.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/glipktzxl.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gadnnktwl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gtraevmxe.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gskowfwjt.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gjbzbfucb.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gdapqsuer.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gxhlcnqof.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gsnrzyxyw.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gtjpjkrfk.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gnazvihrk.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/ggdctbrvf.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gzwqqvmqy.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/grrxjsqrw.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gursuwgxx.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gjkfcdgyx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gbhxwnafh.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gbuogfhvt.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gjejpzsmg.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gtcmcvgjl.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gbnhihuzo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/giodfgqof.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gsbdngxdg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gbbnmtrtx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfjhilvul.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/ggsglmtpo.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gzxprkoyg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gmpvzuyjq.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gvmcvmwfs.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/grqgxtfss.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gpzqxbtnp.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gackanhxq.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/ghjthwuyl.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gcvenjjol.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gurtzduwu.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gryvavbfp.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gvvbeixhz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gugchuent.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gytitkppd.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/ghpyvfweo.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gzmvuqhko.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/ghflzaypa.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gkzdcbmgi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gpuczlbol.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gplcwloxk.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gspropwei.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/goskloksv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gtxyajcam.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gvyidueco.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gzdyaddcr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gotzimmrx.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gfvjiimnj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gofrbngkb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gvsccintd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/goltfjyfz.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/glqsmlqxk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gnubzvlcs.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gowgdbejh.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gasnmygju.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gnddrvuql.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gnzpomgwz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/ggpisktth.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gztpggqsg.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gzwhmssvz.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gdjoybsoi.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gufvvshdt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/giotwllii.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gdeiqogcb.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gfaqlgqba.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gokbtjljs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gfbwynzhg.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gqacpngfv.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gytjjkkpl.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/ginfpkgda.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gqfovvtgn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/glsyzktcy.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gbhtqxpwm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjxlwkamn.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/glxbxlonw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/glojpttee.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/glbytyodb.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gjpuibjam.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/ggnpmbdfq.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gkwvprenp.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gqglqwhdp.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gvcwqejgu.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gmtdgsfcw.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gseskgwfm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gaqdecrdw.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gpuxkwxby.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gqyjabpob.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gstdnfmaw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/ggdoibtme.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/giopbrhiz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gneexaphj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gprummjym.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gmluwwirp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gyfbqadud.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gtuyjotct.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gfdgpfbgc.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gnlewzzvv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gxmgicens.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwpvktgjt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gkoxjdnfg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gzjsjrqsd.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/goxmuiatm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/geyycniaq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gowpyztbo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gfberscgk.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gpyqsdlyo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gdlmtnhqy.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gfiuvtgtk.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/ghxtjreys.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gxnyevrvy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gxrmtvbgy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gdiqbgwty.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gvwpqpiou.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gboxgxioz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmvtnqdrr.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/grljgnjff.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjhfcybxm.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/giitahzaf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/glaofckri.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gputhqseg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gmjptwunj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/getmsaimd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gyandmkau.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gsyaaxnki.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gljjsirbb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gvhianqkq.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gsupkxjqf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/grkwqkxjz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gocdgpnud.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gawxmlzja.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gmmrsuspz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gighkswid.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gcrztmclz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gwiehijpw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gvudraofm.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gxqqgsrtd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/ghiobicjk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/grlqbsnkm.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gjgbdyobi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gqbcstkau.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gmdhmvsdj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gdecowhcr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/givneajyw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/glluxkbcs.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gxpdfjucu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gfedegres.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gaproxdgl.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gcqiutlnc.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gjxfofvsl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/godqisfcr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gcufdnlhw.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gvdqxouad.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gnvpmvjxt.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gyvybclsg.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gmvwqgotf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gqmrsubll.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtzjbgvoa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gznvoponz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gyyhqksry.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gnyznipjd.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gzfzpyngh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gfoogbewl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/grbasaqhl.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gemusnszn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gtvwmsvlo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/goxqyamto.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/ghpwdxtji.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/ggjhpaipi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gkhdmbvdw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gujabdutr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/genkdqydt.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gsohdtuji.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/glvbdysvl.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gqzmhughk.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/ghnahuyah.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gstwxuhlo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/grujfxkej.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gifphlvgt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/geqyogsta.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/genchceag.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/grqglvxmd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/grexqerqf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gqquwzcyq.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gwjcnuhty.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gxrfhqdre.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gcjizakrm.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gvolmfkss.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gbzlchcbq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/grpzhmztz.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gaapuzqkk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/givqkjxnn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/ghrjncpfy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/grtihxzsd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gcigxxdjh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/ggxovvbig.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gtafmjduq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/grhjtenic.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gcuavqybn.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gjulcqysv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/grkmfvupn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gbzxpstfn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/grxgbaypq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gdzhsrugu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gofxbmoti.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gyvqofdhn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gwwixutvt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggkttgxoz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gekcxdele.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gqqelotjo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goulgtjzd.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/guwhafwvr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gcedskncu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gnhseimrh.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gjulfnjgd.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gszsrlohl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gdzsficjk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gripzuota.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gbacdlppj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gokzubobh.sHtML


<!-- 参考信息 -->