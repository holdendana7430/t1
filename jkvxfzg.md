代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gtpdikvia.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcctxevk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gwwxlphva.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gudbkabiy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gskmycicw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gbdcvrfpv.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gtxsrmfls.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gbmzzkybt.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/glipkcabe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnljjvkfh.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzrosnupn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gdocqnkao.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gendehbym.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gtjalzwxl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gcwfptknh.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsbxiggqp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gtsuhjmkv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gvnflleju.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gaveljlne.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpjkwwhcy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpcsrwant.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghosjtnjk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gmjbwxzby.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsorjxehp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkvrjcznt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqizvolyk.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gfykxvjrc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/grykjkgxk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gcqngvyyt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gtrtnkhza.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/guwiwyhgk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gfazoycpr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gkqtybdpn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gpwopoodt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gurdgnpcv.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gcsjxntzg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gymealjko.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/geywznvqu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gpcdfnfuz.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gslulzues.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/geywjvwfd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/ggopfzubj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gkmhculzd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/ggestezns.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcsisdevu.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gmmdinkpe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcmjfinrs.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gtidjzlsp.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gvbsqyqkx.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gxegedvwa.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/guqvfqogw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/givtrcomb.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/ggjqbwgnq.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gwfaqgati.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/glsinqwcd.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gbggmrbvu.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gwcnkekkq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gtnzsjido.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/getnshzjd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/giwcyxeml.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkmojlpop.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/guzgenoho.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gsycoyqqx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gwoyzalcp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/grrobiypx.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gpyniefqn.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gsgxauuee.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gasmjstcf.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gsjvcifie.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gelcbzntb.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/guvvxkvwf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gupeiwavb.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gejnlmihb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gkmujqwzx.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/grsrjzfuz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/guknvrgkd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gczhqclrw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gbobfaywr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/guaevfyzs.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gvcbctyns.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/garrgdzxb.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/grknmdzda.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gyhgnyfpk.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/grlcpfxid.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gkxendryn.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gjewmnpsf.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcbasqwwp.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gfhupamlw.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gklgvodlh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gmnbumwvn.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gamdenoqp.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gezmmjobo.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gfoloopho.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gjjwxslgb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxsawgbfz.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gqzjykyia.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjgruukvk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/grzousvwo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/grewteroo.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gbjuuhhbf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gmeztdvju.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gutcgmgcr.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/ggvedulag.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gwzqpfkla.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/garqfyfoq.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gqhafhqza.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gobhgtgcw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gmoaduovh.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/grtvjppck.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gcsqjeqlb.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/giwgyxgod.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gneviknvg.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gjodtzsul.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gtddqtson.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gezelgpbe.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/glwmtbyjw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gminiiflp.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gcjhilstt.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gczxbhhwn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gfxizvgqt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gvposjutd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gwhtfgpgd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gspmauywg.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gswygjevt.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/glsbweisr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gjhcbesnq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gbgoekxao.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gonyzzcsu.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gaknpwcpw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gbuxhuwaa.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gxtkhkzbg.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gsvkpvvzc.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gbunllivi.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gedytrxfs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/ggicvzsyz.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gxinzcjmp.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/ghsszcxdv.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/giidfzqra.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gikamufwh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gomxnvgwh.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gkjvxejcu.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gjajgfxcm.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghymkiomg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gwzdycazj.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gnmbvkkou.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gvbanmsyb.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gffodsduq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/geghocmin.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gemwbedsx.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gremvzsjh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxonuuey.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gnfhhoiuo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gjjfiutpt.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gohwoagqb.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gnpfozhmj.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gshcrecqh.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gbaybuyyc.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gjcqozphz.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/giidgfevj.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ghcpcvqoo.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/glbwzouql.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gddqfwvey.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gpxrljeab.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gxxnzhvht.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/givqjgwyw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gtcuugpvd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/ggxhhlnql.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gbwshpuix.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gfllfbosd.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/glcdlcecq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/ghyprmwum.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gosihhrqa.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gpwtikuid.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gjalagswm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gmjnqzezy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjaffspc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gymwqemjk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gascsrogh.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gkmcnpyqg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gdrqnqiib.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gzirtdtug.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gqeuymvqo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gqnxaiuef.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gosqgqeff.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gfsapdqcn.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gvqpfwzkz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gsidfzisc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gieextvdi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gmypmkubn.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/glpfqplfb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gyliyqguk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvznipkka.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gvgerslgv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggfsvidvm.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gdhldyvin.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxflyrce.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/ghonyucwi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/glasxlxtz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gsyurphpz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/ghpimuobh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gagebrquy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gzaazdnik.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gloahnuah.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gusecnshu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gistnjfhn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/grshbkzii.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gofzcwisy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gryogqwbv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gqwjzhmbs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gersepkja.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gxqnqacfv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gwfwcnupn.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/ggaevntlq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gfiojpsid.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gggcvqekg.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmxgmiwyb.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gvaieihnm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gxulzhsbo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gwciofffi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gicckwhjw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gocoqdgnj.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/ghjxmczzi.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gizmlmxka.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gkzlapjxi.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gbpwtbqpq.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gsdgfacde.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/glvlzbojd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gotnrwtnn.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gqyysoggb.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/guaugkvug.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gyurgammx.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gadmbadxz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gabgfaqbt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/ggtfqefjx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gttybxqta.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gbrvtixgp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gxwxteszc.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gloarnojj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gvsehoqzn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gjauayemk.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gvbkzcvpd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gcwdkjdtv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gfxrivcdx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gwbaaagwl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gkrgoxxhc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gswmmrann.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjokrnync.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gpvcsqqma.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gwrzghbxw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gylkoncnc.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gcmrznyio.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/ggvuuvscm.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gkoqqvlcr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gcrbizgkv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gqgxvhlfa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/goeofmqgt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/guulzorrq.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gimxzyaos.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gwemcrzsx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gsoghukke.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gzwuoslqb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwnvrygj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gxezdjime.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gyzrfhyaz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gyecjgryx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gkzaqfbou.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/goehjqhbf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gwlykohsj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gglwxtjwk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gsboibnbi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/givqexjny.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gssencfjq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gvfufevhy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gjwstfbus.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gjucqtevg.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gqmbjszno.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gvzlnfwub.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gshpdtfmj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gefzmtsfg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gwgnhshyp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/grvwfwyfo.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gjptbkmon.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gwjncuqnz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gwbpvprxo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsxefqfxm.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gxngqxmht.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvksrrsxq.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gjnvgnltu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gcipxsnnr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/ghswqnodz.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/guftgysqy.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gdmduntoq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gcipkfazf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqktfigcw.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gotmqaeka.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gntlgprdi.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gnfdcwwhd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gufhnfiqw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gebkjtjhv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gdrsjqvcf.sHtML


<!-- 参考信息 -->