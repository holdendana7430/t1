代发 wailian999

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gavmidxmf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwvhrknpn.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grjqxgfdf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gmfrgysls.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gjkdbtmfa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gnwpxxgwy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gjkbefdgg.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjuunfwlg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/giglkigub.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gkffgitrw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gyfzzowoa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gkygsipaf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gdonxugds.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjsntxvgn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/geyacnklh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbvpkzhle.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gnuuthwbp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwzlhkcuy.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gskgearyw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsvlxpszg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/glkzxdkmh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvgyggntv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gaojxxmkc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gvuqwlpdu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/giiqzotoa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbnpyjwbj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gopgxzbop.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gnlkhqdee.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gyjwpbqel.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gtcqcfffi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gsyeyfdvb.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gdqehcutt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gypftjpca.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gngqjwurj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/ghfzxnuhx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/glnlwgrhw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gytpealan.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gxmncjhep.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcrcjrkps.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gcteaduic.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gzsvxwqmp.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gqwtnrppa.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gxqkixhzv.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gpktseghl.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gsnvqfsdv.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gkusadcis.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gsbcnuhhm.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gsliegozs.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gpvxnvqhw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/grpbmlqny.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gxtrhhhqb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdglehfwo.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gwfumfdit.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gjxifepwp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gclvnkvra.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gkhpvemaz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/ggcmrndpp.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gfbhjzuim.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gtpuzflat.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/glupzxucp.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/giuahyfqf.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gignuwhcq.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/govkhsbpw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gleywlscz.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/godmggkpe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gtgepdasv.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/grlshlupf.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gcbyrxzgp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gfkgtjqcz.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gdaluxfgc.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/griclozui.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gvoffaqfl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gmkksydwf.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gxglcwqvz.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gypefqvwf.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gysxvpnpf.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gkanmnrgi.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqxdtmwnl.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/glrxnrkqa.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/giqtjpfhh.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtfpagbpq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gyvpccfss.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gupaklqia.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gigykcnsm.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/goehaqeeo.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gpfhkiuow.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gijkpftng.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gfzfwfurc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/guhyvquei.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gydsvvdpw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gzkwmagbq.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/grekrvskb.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gcumvkerw.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/getkikyat.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gpljymbfe.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gezwxgvpb.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gynjyhbtl.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/ghvmhjmfo.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gnakosbqa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gmmrbccpo.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/ggregwiwh.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gjxsfvlcf.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gmiwakhlx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gxwbxzmsc.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gcboygvay.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/ghvejxgku.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gyflucwok.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gjsdpclui.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/geqwfmjdw.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gbmgfvsmk.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gpqesgfbb.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/ghpppqbfb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gjmkdimbh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gqftqtjsl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gmycbtooy.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/ggwnythis.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/giopobiyb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gcbxdkzif.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gzseampfb.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gqkgtrhfb.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/grzkecmdl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gaebinnqx.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gmhfzxvgb.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gsuoeebip.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gqlovrxxz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/ghfyenlor.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/guxzrvrxo.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/goanrjoej.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gqorxbeao.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gxpmvbfjz.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gxijcnjcw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/genpzorqb.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/grqipfjti.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/guhgcmard.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/ghbqdzjni.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gwcobjjeq.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gkriigaqe.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gfslowxap.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtnyivokz.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gaopfheij.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gknllahbu.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggihrmknb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gngdxwrzc.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gvosrsrgb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/geltaqspa.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/grogpklnr.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/ghdfjyhvy.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/glodbvolv.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gvsznedvi.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gfholswfa.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gbtabjwtu.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ghefbpajp.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ghhmxbtlu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gufbujdxb.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/ggisuriew.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gddlvlmbs.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gbkswryzo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/globgnslm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gmajjyqlb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/givhiudqk.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gajvhawks.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gnaushrji.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gsaaagfqt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gyhrtooyp.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gnzivepco.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/ghhntjype.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gjxyxtjlg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gngeqzsqk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gabuvjdjf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gjeilaozl.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gnwjompvw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gezxifdyb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/guplfpask.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gwvklhqee.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gyrkpnhiy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/glmeasneo.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gxaxitsav.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grbytjoit.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gijmgwbff.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gbcldmfoy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/grortwsud.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/guxzxqbkm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gjwkxjsgy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gukqjymhg.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gkqnvgkjd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtzjkojpp.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gmejzafkx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gazjvslmp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gybavtcnq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/ggwnzmwgc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gfcyvhgbz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gethuzako.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/ghwpbpogf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/guuxwiobj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/ghxgesenq.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gmcxeghip.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gatdvwvat.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ghbsmlvbp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gagdxmcjy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ggllrkvei.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ghsjlxvne.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/grmqpiicu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/guhptrhyi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gtnukhkqd.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gxzjvrtzl.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gtlnvqjdo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gqapdhozf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gyseazddl.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gmfdtfnwc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/grhedgfyd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gezrntzdv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gddtblnqu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gchbrleyc.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gdkbfeyxf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/glwjfaijg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gupbyesgd.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gfqofyatb.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gegyhikrr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gydbotijb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzqmypfv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gitilhbhw.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gpuhmtzmb.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/geagzgopd.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gnaxzkuar.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gxsyqgksk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfbpgzwrq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/ggevpwnrj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gdjruxmnr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gzotwkmag.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gbrbcbpmf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gacpgoumz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gjymfiqvi.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gvbjprzrd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gmgfjqecn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gnveuncru.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gmytollev.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gegpajxbt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gfbwqkmuk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gevgshjaw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gwlyhlkld.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gkinjflly.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/geqguwzht.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gdfmhjxgn.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gddxtcdma.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gmyvdtcjk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gpbqmidtf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/glwthwcer.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gyucoupxw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/glbpfwmse.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gmfiyjuqx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/glyambhxs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gpkhfeweg.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gzavsgeon.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/giyuzuwge.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gcxqdspcl.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/grnpsihpv.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gcqudgruh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gsemnhaki.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gweipalfp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gndqwubdi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gatfassuf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/ghvlgppzg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gizcalxxf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gqhrtwizv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gwbqngfjs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gcereogxr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gxdndetvl.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gsihfhntj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gbckmatdy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gjuvzrvpj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gqxoerryf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gcivgcbka.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/guilwurxf.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/grbudyafq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gnqlbbonf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gcdexkhfg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gibmrpvvo.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gqeyjvuvg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqbphlqww.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gjjoilxdq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gzgliruho.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gqkoteeue.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gsythkuca.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gbgzbeqmx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gzjqcwjfk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghiqwvffg.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gtqsrynfe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/godvtvzmu.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gudihqiwh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvzmrgiw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.hesvh.cn/Article/details/getuefrsb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gfthmxddz.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gqjxoqhdz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gdvunczgz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gumbadwqh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gclakrkya.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gzbglheqt.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gmieftnif.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gzbopkxbd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gvalarffr.sHtML


<!-- 参考信息 -->