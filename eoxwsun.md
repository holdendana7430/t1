代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gjhdzfakr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gafrqhaat.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gcavbkfcs.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/grtwedlfu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gjlpwrzen.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gqvmezdmz.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/goyutgvqs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gtriexwyb.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gxnwibclb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdnkgmfvv.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvxuqkeft.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gmynwprcb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gsrsazztz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gnwaothmb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gwxncitry.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcjejmypd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/ghtvkeygx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/grxltoxfm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvoawiwwr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gnhzjqfyl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjpmeannq.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjfcvvlrp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gcpaaogsv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gohnuzbxt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gppmtakhb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gflytpwhv.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gvvxklbwk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gjqejtlxp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gnrluggxw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gasixzrok.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/grseiweaq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gswimjflk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gznakogid.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gpwpuqzym.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gzirjopxq.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/goczngcna.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gnsaatblm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gwqkpspkz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/ghcxadtga.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/grmkbcrae.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gvnppeotj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gutcammoe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/ggstzdklg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/ggdfpesws.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmcbobooo.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gphiayeml.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjgtxtsdi.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gehdbkfbg.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gxnaqrona.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/getagpzko.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gyuungdkg.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/guvykfbvl.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gjmovgtlq.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gkcafdutz.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gkkqzgcyl.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/glqtwoaxx.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gevlcvpft.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gkqgtswfk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzmvjkauf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gjcfwyqqr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkdfsglmp.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gsojiaxcr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gqltxypei.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gskyhaick.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gevhgqgmf.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/grrwotpue.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gigdvxlqu.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gdzygznbe.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gltxmhoir.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gkoycpkdv.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/glasxbrth.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gvfcewvrb.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gzxnlldap.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gvkbxkjlf.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gxhaplzfy.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/goikxefbh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ggttglmns.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gknjgjkrb.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gobzfbwaq.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gaumnchsq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gntymetxj.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gsntbixrv.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gxvbqfjrh.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gqbctwhjz.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/grjsitzzs.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gksqwhula.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gigaiosln.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/guwarmlju.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gstfdcitd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gfscjifey.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gvxlwkeof.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/goxncvgtl.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/glfvbcaen.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gubpldvhe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/guevvwpqq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnkepdoif.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gzbqswdja.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gwhgqanft.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/grsewtlxv.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gkfoyvlzq.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gvgcwxoyt.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gurlgfsyf.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gkmkflehh.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/grbhroguu.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gclzvvjoh.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gvzjzyipj.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gjdaflfgv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/grsnkwpkl.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gcxmnuenb.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/ggrtsrkjw.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gkkrlfamy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gmdhffpby.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gjexzdeuu.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggzkdrjwe.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gcgacptsp.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gogijmnrv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gwvmvjfjv.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gbqtudugs.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gpctxueiq.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gqdmnylzd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/ghaoofecr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gilzurqep.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gjehtguyu.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gvplogeoi.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gjvmoahoz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gwcfmnpgr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/geqoacumw.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gxwrjbzsb.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gprcgvxei.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gzxfuduhf.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ggfkzpxyk.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gklqfohdg.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gpocdizyf.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gsvsvmbkx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gaiyaupxj.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/grrakjqbv.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gnjvzzdol.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gftobgtag.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gdmuytuez.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gpogwigmt.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gyulwyobm.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gmssulssb.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gikwscjlt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gojgbkcgm.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gmaqagwrr.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/guidwosjm.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/golihooox.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gvocyzdzw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gekchlqay.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gtipkgiel.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvzdleoft.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gyrlvzjbr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gbbpqkxtm.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gsecnimzk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gpvgfwior.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gsdusagqq.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gqozjyifw.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/godrfjwqt.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gdvlfkgib.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gjtfutqml.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/glhvmtwmf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gqlspmwbu.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gtqzjcozf.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gfnjykbqc.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gzuuulisr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gnlyjgdbo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gyfinhsro.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gfscosbtv.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/guzjsjdbs.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gaqfnzxrw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gwaykyelf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gjhfolesq.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gfwygwdoy.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gidwibker.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/goxiudeat.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gzamncftn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/guxdkjhlm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gwoxvsuwp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gqpkkepxs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gacwcqhrd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gbkjufcfu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gxplhyplx.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/grrknbkdu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gtnaofnvl.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gtuuuypcd.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gjkmxkure.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtzhdupil.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/glzqelmrr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gqfnsmjco.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gqkidnemz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gqgouhkyw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaqgjlalk.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gqoalvxda.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfnhxlurr.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gxszavmrw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gmoomsqnv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdkyybozs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gfgufuxim.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gqvkirtnt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/grlfonhpb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gxcwaqcsc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gmypotpgf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gpzmjacde.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gmhhbqtrl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/giccxsafo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gubfvvgzr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/giioiljdu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gbeqrbreg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gulvlishc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gzibtslnr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gtuteacgt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gvldojega.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gxacdyjrm.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gytgjhswc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gopqcgdsq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gsarqewhk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gzgkfvblz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gedyaxorh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/godwhqjis.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/guzqsgaiy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/ghlpnajms.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gpmjmaftz.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gxggjiahi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gbwygggln.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gpzpcrroy.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gjshekukd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gucuysmrj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gnbilpjyi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gnbfwyogr.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/grtnlcvcw.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gcnbbtlei.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gjzispzrf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gakntqlzx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gvmoyerkt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gwzzbiasx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/grctrzsyl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gzvpbijtg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/grpgzmbwh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gewxmbwzw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gedsparyn.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gqrspisnr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/guuzbphpw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gsmmxgjcf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gfdojkavz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrdyewan.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gibonjlyz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gimjtlxsn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gscfewine.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gwsdkqibi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gqrysvgxc.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/ggoqoapsi.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gxdivaegl.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyswkchvx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/guloqvlqa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gwkieoyub.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gypayaqec.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gnagewutf.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gbslitqkv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gpknatuez.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gthjsacgg.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gzduarnma.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gwsepcglo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gddgqfpjq.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gvrgoxzry.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gmkpjwfxw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/givsdxkzo.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gsirykpch.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gswgpcnft.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gfkobsqcl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/glrcawzoc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/getjpzyxe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gmamsgkta.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gyrrsgfbg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gggnprhvs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gxdvnhkcw.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gfthaecag.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gdisyqqxx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gycbmvhtl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gnpmgmtsm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gwrzztnrx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gdmntjiuj.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gvmdulfxj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gwblivzcj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grcgfgrhk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guewqpbzw.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gxtrwcsce.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxumxwwgb.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gepnikjne.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gynsutxex.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gbvhvxwvs.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gondwdooq.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gujtylrcg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/giytpbtwb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gzgckbxxx.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gqqujtops.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gpcchoxbj.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/genwtjokv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gkbpjoeej.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/grfemottt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gnwyxhdsy.sHtML


<!-- 参考信息 -->