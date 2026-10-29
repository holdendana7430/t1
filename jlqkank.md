代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/glukdzpbt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/grigbjflc.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gebgpabsu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gbwfsurmt.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gnzrdagih.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdhziulwu.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/grmnpjfbd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gbouqlkty.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gezqybsih.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/grblmzons.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gmrmcrgpd.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/goqdufyje.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gsjzxahmx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gyynoqsgx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzcyslqrv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzvyrzaem.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/guybwydut.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzbrrgfmk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/ggrhgsbrg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdeivdolr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/grnmyvanc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gypbjgqvd.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/guqzrcior.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gzcczkzzg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gkuhfdfof.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/giaritpjp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/govtimmwi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gyaghrkds.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gydhlnbzt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ghnjtelfg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/goqkyeaxv.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/ggbxdtlsm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gjukszleh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/goznkrhsz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/guvsowptt.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gvnawgved.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gsdfxdtux.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gakerdlgj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/ggbzalred.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gblmhiygq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkzvouedg.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gnlpmoibl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grzmkfktp.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gyobrpizz.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gsehkdwsr.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gdmmpwlmy.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gorzwanok.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gvvkyaput.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gukemsptn.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gzgpmsuvd.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gvxiggbjc.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjnlpbuvz.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gyeitrcjc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/glkisgrvg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gplyamtpq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gdowhagqo.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/googcdqwb.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gxknrqpki.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gjnlqwjob.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gsashkzlz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gkioocgah.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gszamuiwg.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/grmxdfinj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gqivwcmpw.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gzlarngpj.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gkmofefxn.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/glfxsejbf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/ghusajjqd.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gcnadqfva.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gzgdfdupb.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gzcopurtb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gwkgzpswm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gofybfpok.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gmidudhtz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gnuczfynx.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/glnwijoeg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gwyopehwt.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gwvprqfhy.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gxatmwdkn.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/ghkobsqno.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gembozncp.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gibuobsub.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/goymfedwy.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ggvwqbmps.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/grleljlkm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gpmqvijum.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gjuxldpmb.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gjivwtruq.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/garxedcjn.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gevegajlg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gaebuqhfe.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gsszzdkms.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gwotteznz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ggudwonys.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gsuqpdkqu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gprcjzcyv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gahhpytgz.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/ggqpgepvo.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gnakuhtym.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gisjgvgju.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/goubewldo.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gbbjvblib.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/ggnkougrf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gvqtiowxr.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/grhgvvfuq.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/glvfdyzue.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gnhkjnoup.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/grqnkqnhu.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gxvpxcbmv.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/ggohubkfe.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gzhdafdfp.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gnnaxtauu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gpfoetkeg.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gvbekwrbz.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gyxtnerat.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gavmdutsp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gdhqayiob.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/geuiqaljw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gynyydiug.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gkfhzxgdb.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gzvwdujdu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gelgeigqg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gqgspwfzh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnwwsjhh.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gsrthsvzp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gkdhabpbm.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gepecfyqf.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gmmnrfqte.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gqccoqaiw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/ggdiuomkk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gnylmzyks.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/goofdmxik.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gbwigizuv.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gdwcfqbfe.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gucjvvhva.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gfbswvzkw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gaxmvhmgv.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gunjvxtmq.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gdivlivrr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gdhlufglf.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/girnvorcg.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gpjempkeq.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gbvedznqp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/guffleumu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/glskgnkhh.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gkmmwhqcq.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/glujyebpb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/goenprdar.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gwbbyqdpi.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gnteedsip.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gbsvnkrty.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gwlvlhghp.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gaqwszkdq.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gpsvzexkt.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ghbcnfovg.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gnfewokna.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gmtmliyvr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gonvblzmy.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gkydvaxwb.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/goedidcjf.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gdmiewhoa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/glwersrxz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gxstjhppw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gipscgopc.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gfgvmvgyw.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gadzhpnnn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gvkubnbbv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gnfnzqkoo.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gbuyxztsx.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/giijripqu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gfbjfvuov.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gugmrqbkc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gwczzmgwa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gnitrnbgm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gphqhgqbr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/graujlzvd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gzopzojym.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/grgphysfd.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gnxirunse.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gbxieitdy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gemwelgqx.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/ggdkwkrqz.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gaaslzpyv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gslmaypct.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gzcsshyel.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/grivjxjgl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gqslgmyle.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gssffoqvd.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/ghvtfkkfp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzkqosckp.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gkypggcnl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/goccqpfax.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/glgcvzbxg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gasdfxiys.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gyjbsclyo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcstxnynn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/ghvkxfnuj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/girsshjnr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gwjzrshgl.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gqmjeyvsl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gvsxckmpq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gsdkheodm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gvjgcyuxy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gtjucsgrq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gioslwxch.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gafqjlijw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gldonftkm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gghklabke.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gdcgslexc.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gygybbopf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ghnkmsxij.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gsecczous.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggaqrgdhz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gnumhasyv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/glxkgqerq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gwlqxvpty.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gnsljpvhp.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gezbvrlnr.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/glimcgkrz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/ghovtlokm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gmfszrmyz.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gihqgmtlz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gnecfcaqj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/ghoppojjl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gnhcybvyt.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/ghiwfurdc.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/ghuujzflu.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/ggydpfpxa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gyequsleo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/glqckinqf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gjmscnrza.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gwhwxmzfa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gfsvkqaub.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gpcpqikwx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gpkkunqlj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gxrujupip.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gkxvbyakw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gutinluwr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gywupiadu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gsrnmgpys.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gcjrabkyc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gatwnebho.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/ghirfmdnn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gyxblsvnj.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gxnygkmsf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/ghtxbtcfv.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/govniozkj.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gszrdxfrd.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gekgpwxmd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gnvnkrpip.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/geeqbaxuq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gamuayobq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gyucwscat.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/ggkjkzygj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gssibhkug.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gflahgyyz.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/girrvxzmj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gcpguphwk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gbqgnafxx.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gcposeyny.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gjxgnjsaa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gjvunjqwt.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gdalnmkst.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/geklafslh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gahtlhzbj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gmjvzcrbd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gzckktxcb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gviomoyxn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gwrqrexbs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/giwyfhotx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gwfgztmlz.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/grqtklvbg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gxqhebfhu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gjlhtbgdr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gvtgzctjh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gkvqvhsyz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gwkcalhpo.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gmqrapwlv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gcgrmlohm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/guztbwesh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glqyulpca.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gkbcyxqfq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqblhxegv.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gaupvbkkq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gjakrrmxp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gkoolyaok.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gsumpbcgs.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gjksghwqw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gxshzvray.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gbcwzrost.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/glxlvubqv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gdkbbrisv.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gseokjeop.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gfwxgbydj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gvgvfhqcj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gbafleiiu.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gkgkmkikj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/ggcdutqah.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/guqdwhaaa.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gmwmbmjfc.sHtML


<!-- 参考信息 -->