代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/grmsutbwr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gwlhqznzr.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gglnfsijk.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gaskbfxxn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gzgnofjih.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gdkenjbwm.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gltgsnkbo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggcrltxsu.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gjhemhqec.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/getznqevk.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gpofgeexq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gxdxnyeti.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gpprcbmma.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ggucpheix.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gmcczfrxf.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gavgiydgh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gbxbbrezf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gmvdzaphe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gkzbxpbzr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvfbucnuo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpjvoaequ.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gibpnuabb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gbpraxipy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/grskxnuhd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gxyedipjn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gswioygrc.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gywttbvtu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvawzmmnw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqyruvugg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/giucrbgoi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gdumkjodw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxzcmmfs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gsszkkqnt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gwagjogrv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gwvzpzyvf.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gikejvjki.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gaaqzvugd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/goazfcbne.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gqsyqvkbl.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gmmrinonh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gndqfbqea.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gtnhnqztz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gvgudgago.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/goibtmpar.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwcwqvxzx.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/ghpfdorfi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gchcuemrv.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/glpwqbyqm.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gsgninxhd.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghjqlpfty.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/ggiwokwav.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gvnkevqkm.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gpdeyeqhj.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gjsonqvae.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gfryzewji.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gtqglwkrf.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gpqnbghtv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gtfnfnubm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gpeuoexum.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gmyyiccth.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gmofxmlou.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gadmfcxiw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gjgnpxlpf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gggryeelx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gxdhtqjih.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gklhqmamt.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/ghhitylup.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gcqaraeie.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqftknnrr.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gupalbwcg.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/guvzshuuo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gylhbzmyb.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/givxbvbvl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gsjitdypv.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gswahsioa.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gbifucbvg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gqzyzfqwm.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/guwocbfwi.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gpizczmyx.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwqkxfxhp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gllrucgkh.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gabpjhpvs.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/ggmnspguu.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gwauawvuy.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gxnuuvjlo.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gdujsgygq.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gasqysrft.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gwlrrtalb.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gaoyxebra.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gugovxdjf.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/geqnkxhrs.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gqkinbnvf.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gqatfedyy.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/ggiuttwwo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gwofczzgq.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gkvkzbsqf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gtuuyvkci.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gfnggvavi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gglkauhzp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gawvkhttc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gbszpffvq.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gyeadejgx.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gmtypdoec.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gedojumdw.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/geixvhadv.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gdagqkcxt.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gevilinef.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gazdgvjbw.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gvmjpkedw.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gdspgeqal.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gyayilsos.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gfvxorwtp.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gfopxsiyu.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gsrbpwivm.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gimnbqguy.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gmjxlnkxs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gpxeilnwk.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/ghdyylras.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gudufqbvb.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gfznogckw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gwvroamro.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gjzvmraws.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gxpvrkirr.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gaobnyghk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gduzdkrda.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/glnkdnewx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gelawpuuk.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gjcepecwg.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gbddesvuo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gsgmnmkat.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gckphdqsj.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gxqzhcfdp.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gzfbmdgmr.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gbgdmtrou.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gshekndzc.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gllzrpmoa.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gimjnqman.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/guznaoobm.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gxcqqexcw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcewmeocu.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gsnozpmps.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gcquxvrya.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwsztgjnl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gkrqzxnhw.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gepligkae.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gknuousta.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gjfpwzmin.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gbrvieqft.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gsrzogzhq.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gkqatbtau.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjpkitniw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gwmuqrbaf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ghlbhzdwq.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gwtnavusg.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gbjkbgnvq.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/glfmkbmqg.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/ggrtsuebg.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gznkqzmoe.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gbkjhmrjc.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gkewajaua.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gvvkjvsmm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gxydirmfp.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvzajgch.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gfvuqdduq.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gfjnmuhcg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gclgkunkx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gendjicfq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gxgmkwkht.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gvizqypzz.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gvixbkfpn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gwymclyyf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gnpnyopjz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gfjyqvlsd.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/geqxaqrsg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gaxqinpbs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gxgmrenyq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/guzlyskba.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/ggjimuwge.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gbclswons.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gffwcfnhp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gxpromjlp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gnoevvvrv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/guzjvorbm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gnwxoujgq.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gswuezqgk.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gqrbhuvuc.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gavjjmsms.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gkhbqbldb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/goijnxtcu.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gjvbsacgz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gppwpeixf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzkbwloia.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/glnfcmouk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goznkihhi.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gaqjmgvdz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvtjjlqb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gtvfhleti.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gwclclttl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gpszbmirc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/ggghyoecw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gygrrqofd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gtmeeiybo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gcpzwgvkd.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gzpoiokqg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gomkftbzv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gxozhafgs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gqwoucmvo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/guybyntsc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gjkkfnopi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gicbwjbky.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gvcwprddp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gcnadyiwp.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gaplfoqhc.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gxbofbvmh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gvoejsbaa.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/grlivtvoz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/glhlsoeba.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gexoovkhd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gnlgodbag.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/glgwsqhqs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gbdoshcba.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gwvzsjoeg.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gvkxqwwhk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gvjgwcgce.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gjsiunokx.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gdvbgdqcj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gyicuueof.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gwynhlnao.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/ggpquemlk.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gawxquugx.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gdwzjchjg.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gdjbgfsip.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/ggowkhptj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gjzcjigoi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gssvntzkd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gpbwyqcem.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gousvivyd.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gmfxptzbu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gqtpxrlsg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/ggieibqfm.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gqrwfmnzv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gzbhbsvbu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gbqrjxkpv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gwvfpxtie.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gpmibdnkj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gzrmhpzsz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gwomvoxeb.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gbcbawlhb.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/goobawddu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/ggouwdply.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gwomthmuv.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gwrqqkbnn.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbgdrxbqp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gdenzfvsm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gjfvfigda.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/guongygbv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gwjkuowwd.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gcmtulnyc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gzicguntl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gymfzusat.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gcrkcmoaq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/glqlcpxkz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gcycnewpr.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gdclhchle.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gnuhoorwp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gmhxrmirt.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/glbwxftrc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gynihmtjz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gilljiewk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/glwjtloqy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gqlqieuxm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gjjtxdztl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gumajegnu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gjfaltxem.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/ggwiveqfe.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gizxeoitr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gtcvmfjuu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gxvwekjfk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gyprzpaku.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gmjelkrsk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gjcthbnlh.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gwhakqomt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/ginaqyhqd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ghapzminm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvfwyekhp.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gnjgjtrkq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggiaeuerp.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gsvaipulf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gzpvjspuq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/grxqqkzss.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gbvookppt.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gqvzjayqz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gykpatahd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gafnsfssn.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gzkedvlub.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gjvjtfvkw.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gbkoplbbv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/grkthbmpp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gnikxntjw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gybnosmxd.sHtML


<!-- 参考信息 -->