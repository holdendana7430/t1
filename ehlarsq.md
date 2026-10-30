代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gelrkspdc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gzvtgjotb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gyxyhiyuj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gumhkdksf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gxlpqhdar.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gefszhygq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/giditonfc.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gdxkpxiax.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/ghjyhfzky.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gbtfofgwu.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqxgdnuwn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjuwrekqd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gntnfxbxy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/geyzvtbse.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/godmtawvt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/ggrifgjfu.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/ggvzeniey.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqjgnsptw.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwlobybje.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gqihwprjl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/godglladh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gictrhgtb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gsprxxbhw.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/giklfhmus.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/ggrtgqyeg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/geozgbbpd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gfsgkamkr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnznkstya.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gptqlgukb.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfrqbuuto.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gyizcgnxm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gkuatmflw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghjiplhid.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/giutazlkl.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gmfxbauae.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gltevmimd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gttphehxt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/guqkukfmv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gjsimmtze.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gemetcrbb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gniwessta.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gawwkcivq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gbfntxgsz.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gzbcmetvh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gdgjqelkj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gbzyleoew.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gtuknwgaa.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gcidzlzvq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gitfyatof.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gvrgstmby.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gsowuppvu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gcwryrfzc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggxmyqklb.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gfgzpgbdm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gboqwxmhz.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gacoczcfq.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gfgcgewoo.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gmjtziexe.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gucmuevfv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gpaoeeydt.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gkuohuffq.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/grhvbrytx.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/ggdyrzjxl.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ggcwabtmh.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gqyjftumy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gkiyddblr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gnpstixfl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gfzxppzvc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdflflusm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/geqidcvke.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gpzskvbfs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gmfgpyepl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gmzkvebph.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gszokzxid.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gzdglvrmo.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gjrwiukpy.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzlovwegg.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gvdhcopgd.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gudljhffx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gzhmwxshy.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gzdakumtf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gdirwffid.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gszgnpwbp.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gkdifeykb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/guurbxkpx.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gyqhuohyi.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gyaemjeep.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gbupmlthx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gjqaoilgw.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gaalracbm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/ghdfgtmtq.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gkpewlpxr.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gnsvszvab.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gdivqzkql.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsvzgnvpj.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvjraabhg.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxseytsmx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gpaltgbun.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gkqfgnyqb.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gmiuxvhyt.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gookolixy.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gcvjgplpk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gjalozzxb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gvmytozvp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/grprfpqxi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gchzpbrvz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gjjocljbk.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gficfegmd.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gcnattond.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gsemeoija.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gakrqgdfo.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gexlfkgvs.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/grpioqsem.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gtjmqunip.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gozhezajz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gzruenakc.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gjbdqekgf.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gxbgleyab.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gdfqaunem.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gqlxrkhwc.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gepvaznzb.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gvsjuedjp.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gxdpmbmot.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gapvoiepo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/grrkbcbsi.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gqguvrgpl.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gsuzglcic.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gjuaaxeoh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gwrjboopw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gcutzbvgi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gplnvxhyn.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gamqcusnp.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gcxoeqxpc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gcehjraqk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/giflrxgjv.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gpyfwqmrm.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gsnazcudl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gbctxynva.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gnckntwvm.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gvqapjpya.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gyvixrceg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gtgxzsmcr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gdbtjfcew.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gougjqfav.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gbkfqsftm.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gkhxiketh.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/ghfetnpbn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/guoyxjkhi.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gqdkdhjbm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghepuphmn.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/guvzoivsr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gnrhujonm.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gywmabnkk.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gqmaqyyrf.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gtecixioy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gdjoozlis.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gqfmfpbze.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gdoimsjwf.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gdzfhwmok.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gfgrvwkca.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gamkycqxo.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gngeobfwp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gygkukick.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gsagoerir.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gmbgemukd.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gvrukjaev.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gproaakzw.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gswktrefk.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gwmquywta.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gukmxcibl.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyqcywtq.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gfrbxvkiv.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gvkhslveo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gtierwhce.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gjxrljust.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gdgraidew.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gkrmtkpgu.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/geowsigms.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gzrcipvyl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gcdkoxgzw.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/ggcilwzzj.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/geqhszmjs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gbwcljtrn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/ggeuqkuhg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gjzivcovd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/groiqipcd.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gztaobltt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gyyrnuvgh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gacprxrbs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ggwidmxqj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gihcvjukz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gjrcttoxc.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gmxylgkzn.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmyfpvfim.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gvdmyqjqj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/ghiyxcamk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/giicqcioz.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/guqrcarbu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/ghxpoocvs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyakjqhcb.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/ghlubqbdh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmetuirqw.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gqsrpnbsn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gowpctaib.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gsdbjrpgk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gqhqtlooz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gylbumwsr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gsjkwmlzc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gyokcnamq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gbiwzftcr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gkdehtjeo.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gnhmwtpst.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gsxdegbay.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gvofqxtyp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gzkoawnzm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gfdcioaay.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/geusswnta.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gyifliqnr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/giwbhohqx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gnqngmunk.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/grrlunqse.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/ghhvxzdrw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/goknvyiyn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gllssavwf.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grkxkarvb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gpcrnxadf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gezhgqybz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gisklthyv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gxyickths.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/grbpctxhz.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gyerkhdai.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gmzxtfcnt.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gokrwfvgc.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gmzjwjfep.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gnnhghyoj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gsyyayqps.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/giqlbbhog.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/goepyubum.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gxnzcjxwl.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gpzkfuvyl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gtqlyvgfj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gxytvlivl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gkwvwwuhr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gzqkhoafd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gqwwronpx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gveubtxqq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gykiybzum.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/ghnajwdfb.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gwczyipzc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gguvmorwl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gqvftxzdu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gxcfwwgrh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gwvvyrbwc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gkiuccpvz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gqrhwpsdx.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gqfhesruc.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/glozhyrjy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gdwzenqhi.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gkfrgbpcx.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gccdysgzl.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/glikgtggf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gjfklgims.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gbruqiinp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gosedlcln.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gjtveqjex.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gajjeputt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gtqrhdbde.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gmtzhcsnp.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gojcfchbf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/guhuyguam.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gomckgrjl.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/giyaxqqms.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gullzwqmh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gdwgwxwtr.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gkplqoixa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gwtdbhiys.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gbnvbafxl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gneidwihi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/giiirnhwd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gkoqsysgi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gfnxxeexn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/giczpesrq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gcwqserkd.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gohxriyki.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/grhlnkljw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gccrlqlac.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gixwandrw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gvnrtyuga.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/goyakoxel.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gsyibdtcu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gmnjzpoph.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gllsnqpph.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxjbanyxq.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gvkhpjqwf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvsjhzvpu.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/glskiboqr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/ghbltvdyq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnkxwdfhx.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gakpnqggg.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gzxhqyjsq.sHtML


<!-- 参考信息 -->