代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/gxtrasmmf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbekssyz.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqgckmgn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gzshhjolc.sHtML

[F09] 获取文件大小
来源：http://blog.fanxiaobao.xyz/Article/details/gabjqbrfm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gkbymjghi.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzozijyro.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaagxikt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjwhdjjq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmflybboj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fanxiaobao.xyz/Article/details/grpnrmqnq.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlqcxbey.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdxgkchc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fanxiaobao.xyz/Article/details/gknuipxbr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gebbftdhs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/ggvlegjxu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtoupxtmt.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gozufgjiw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgwzuzlw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbzfygzm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtvmarth.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gmztxsvep.sHtML

[F11] 复制与移动文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfnclrbuv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrrlqqbr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gequrmltx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzuvaxkf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gxzpooyvb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gwmissmew.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/gctclxwdo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnxbrqqf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqgrkuig.sHtML

[F12] CSV 读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmvwrzxi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtygiaqiu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fanxiaobao.xyz/Article/details/gnquiohpr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fanxiaobao.xyz/Article/details/gtzvrslgs.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gftxoxmnf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqjpuxqf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gocomqegy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmczmhvpx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gpucnnodz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gchqqvblm.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/ggrbyjprt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfpeayfk.sHtML

[G01] 定义类
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpalderb.sHtML

Py:   class User: pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfouchvlh.sHtML

PHP:  class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjxeoynk.sHtML

JS:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggppjrplz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwndfijpu.sHtML

Java: class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxpetkzah.sHtML

Go:   type User struct { Name string }
来源：http://blog.fanxiaobao.xyz/Article/details/gfurpantj.sHtML

Ruby: class User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkchnyrpg.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvoaiagws.sHtML

[G02] 构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goubmptra.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fanxiaobao.xyz/Article/details/gmgjomzos.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gsehffqpo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxudnbiu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grneweixk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfcaxijj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdfjuzxx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gexietbvn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giigfkicw.sHtML

[G03] 实例属性
来源：http://wap.fanxiaobao.xyz/Article/details/gshebmpuy.sHtML

Py:   self.name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gquyuejla.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfaypqiz.sHtML

JS:   this.name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gthcqmkwr.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqbkdijh.sHtML

Java: private String name;
来源：http://baike.fanxiaobao.xyz/Article/details/ggjeimyqa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fanxiaobao.xyz/Article/details/guencgdma.sHtML

Ruby: @name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfoupqbu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/grjzpmome.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/grzmfqeiv.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvhrkhyv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltusozfc.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggvqqrnyl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcekgpli.sHtML

Java: String greet() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gffnmwqap.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gfecmbocg.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gmijsxjui.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gflukbcsl.sHtML

[G05] 继承
来源：http://wap.fanxiaobao.xyz/Article/details/goegupyyz.sHtML

Py:   class Admin(User): pass
来源：http://3g.fanxiaobao.xyz/Article/details/gspotxwvx.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplrfgcnb.sHtML

JS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwbmtggky.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gghwqnoow.sHtML

Java: class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkvwhpzea.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpaguvok.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmoyjvia.sHtML

C#:   class Admin : User {}
来源：http://wap.fanxiaobao.xyz/Article/details/ganlzogkt.sHtML

[G06] 重写方法
来源：http://blog.fanxiaobao.xyz/Article/details/gmniiekcq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvicllqu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnsnfufz.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqsfhzmkm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwerfplvn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ginumdbts.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulgwlpmc.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsaggfxk.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwcgdjjm.sHtML

[G07] 调用父类方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gymgcyiud.sHtML

Py:   super().greet()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdnojzwe.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gnzixcvrc.sHtML

JS:   super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gjxwbadqf.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtevshqr.sHtML

Java: super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gtsulrjei.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gqysnbfmz.sHtML

Ruby: super
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxfoztpy.sHtML

C#:   base.Greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtdjqopb.sHtML

[G08] 静态方法与属性
来源：http://baike.fanxiaobao.xyz/Article/details/gqmuhepye.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fanxiaobao.xyz/Article/details/gxiomxlna.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghywbniuq.sHtML

JS:   static f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/glrgbjxpj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjvwgdew.sHtML

Java: static void f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gczxkwjqx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxnmejau.sHtML

Ruby: def self.f; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzrivoxb.sHtML

C#:   public static void F() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzizzarug.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqhuutlt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fanxiaobao.xyz/Article/details/gdrgkltjl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjdlnbsya.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fanxiaobao.xyz/Article/details/gfdhcoriq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgwsjeua.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gundvoohe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fanxiaobao.xyz/Article/details/grnumqwlb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydrxjjoa.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwwebkms.sHtML

[G10] 访问控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gdonacugi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fanxiaobao.xyz/Article/details/gznnvxpnb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdwzvrfe.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fanxiaobao.xyz/Article/details/goziwzswt.sHtML

TS:   public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gonkwawwq.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fanxiaobao.xyz/Article/details/gkrvzrbah.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fanxiaobao.xyz/Article/details/gysfcnpof.sHtML

Ruby: public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/griblvlgh.sHtML

C#:   public / protected / private / internal
来源：http://blog.fanxiaobao.xyz/Article/details/ghioqjeyd.sHtML

[G11] getter / setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmhuvxlf.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmfdmcld.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgcmlgni.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwmphiiw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjtobmce.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gespkndni.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gygnrllqt.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/gkthugenv.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxdcclfb.sHtML

[G12] 对象转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/glnoqkkbb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghadrqmlf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzlhielc.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxjhsfyc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxpvixpf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzgdiqbf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzawgjkgm.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcflcqkd.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gwrwgdeml.sHtML

[G13] 判断对象类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gninqneiq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqyulyaj.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqwakccm.sHtML

JS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gkofbqesz.sHtML

TS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gyhcudtnm.sHtML

Java: u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gxsdphagb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzdqavzg.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrocrcxy.sHtML

C#:   u is User
来源：http://www.share.fanxiaobao.xyz/Article/details/gtozbptkc.sHtML

[G14] 数据类 / record
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqgiavya.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fanxiaobao.xyz/Article/details/gcrfuyimp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fanxiaobao.xyz/Article/details/gydmwlfjn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsneqgcle.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpflrlopy.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtucndlma.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxzdzpzk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyalokpkf.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fanxiaobao.xyz/Article/details/gxewqqyxa.sHtML

[G15] 枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqebcyqup.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyuolntx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggiatqhby.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fanxiaobao.xyz/Article/details/gceldbejv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gzqvaysze.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fanxiaobao.xyz/Article/details/gjbysnxxu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsiirwms.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqwywvjw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdhlrkbc.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiahqqsm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fanxiaobao.xyz/Article/details/glxljkwom.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnunlcpy.sHtML

JS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gqyrmeshj.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsfnvzwx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuadkfuz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fanxiaobao.xyz/Article/details/guihjzjfp.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmktxwlkh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstinjqun.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggegxxaeo.sHtML

H. 异常与错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gjvtowmax.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwycvubad.sHtML

[H01] try / catch 基础
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpvenzvc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfnaombi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbkmojzj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwoahmczq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gokcrsbaw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmlkpfuo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fanxiaobao.xyz/Article/details/gdlyhthcl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fanxiaobao.xyz/Article/details/gpqiwgwlw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqexwnizh.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjqdvnwd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtetegmt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwuajyej.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsdbknqw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtjbwcng.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/greigfdgh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjherhqkp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggighlimh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxeytivur.sHtML

[H03] 主动抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gaxtlyttg.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fanxiaobao.xyz/Article/details/gehgwoiur.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtswyyiv.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gazirqxib.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gpzjpixry.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryoharny.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/gqnbiydts.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fanxiaobao.xyz/Article/details/gytvschch.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gdslhguhn.sHtML

[H04] 自定义异常类型
来源：http://baike.fanxiaobao.xyz/Article/details/ggyzzlpuh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzflunfg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grogjaoks.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkqlqbuyb.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfibdgjj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpesqlkmd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fanxiaobao.xyz/Article/details/gzzfntzup.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuoowgpl.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgzkrogs.sHtML

[H05] 捕获特定类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grzqicmaf.sHtML

Py:   except ValueError as e:
来源：http://blog.fanxiaobao.xyz/Article/details/gikbhagwk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fanxiaobao.xyz/Article/details/gqngygcsm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxdcfpvxd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grtadplid.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpipgdhcj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwosvlox.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fanxiaobao.xyz/Article/details/gqejzywgs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnulnpgi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fanxiaobao.xyz/Article/details/gszowwhll.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fanxiaobao.xyz/Article/details/gruinmqua.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghncdjhdk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndbmitqh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gvymutaoo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fanxiaobao.xyz/Article/details/gujhysgvz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fanxiaobao.xyz/Article/details/gbrypnbbv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtubcwgea.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggroxvbwp.sHtML

[H07] 断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqtuvovt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fanxiaobao.xyz/Article/details/gtyqersnh.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/godpdcoyc.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gierdznpd.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gfpnukyme.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqbeszkh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fanxiaobao.xyz/Article/details/gzdpijnuw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxybhxmc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gvbepncec.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcxrmlfe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fanxiaobao.xyz/Article/details/glekmqwyf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fanxiaobao.xyz/Article/details/goprwquog.sHtML

JS:   e.message;  e.stack
来源：http://wap.fanxiaobao.xyz/Article/details/gbsegffeg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyebxggnv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fanxiaobao.xyz/Article/details/gctyajsae.sHtML

Go:   err.Error()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqqhqgyf.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fanxiaobao.xyz/Article/details/gkxbnlaud.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwpehsgs.sHtML

[H09] 带错误码的异常
来源：http://wap.fanxiaobao.xyz/Article/details/gacwxrute.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwwjhqbc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/guozdkbdi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyiiumzf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjwrjihf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfoheusgh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fanxiaobao.xyz/Article/details/glnequtpc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzxvyrzk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fanxiaobao.xyz/Article/details/gkugqizdq.sHtML

[H10] 资源自动释放
来源：http://baike.fanxiaobao.xyz/Article/details/gygedbebx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fanxiaobao.xyz/Article/details/graiquorl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrgbtxbe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnnimpdi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhiqywic.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/goauurkwe.sHtML

Go:   defer f.Close()
来源：http://wap.fanxiaobao.xyz/Article/details/gcabstera.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioskyoqm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/glfnhxaht.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnebtaoso.sHtML

I. 正则表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggximzjqt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfbptqexh.sHtML

[I01] 判断是否匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgxtdtjg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdmuhuie.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdnygylq.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghycyxvmb.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijiklevy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fanxiaobao.xyz/Article/details/gqouksuol.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/geezepiwz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghujgufye.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxtasput.sHtML

[I02] 提取所有匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjcdvoej.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganpdrtfo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/goguyybkz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjmbttcf.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuwbhqqj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gggztcivr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gpzaqdwhj.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gijiladbj.sHtML


<!-- 参考信息 -->