代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxdkenige.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gudpqwkrm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grpzodval.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghdsrkwsv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjzuzleop.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfaqfiyqj.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gjbclhoou.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/grvhxzdej.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/grigyxfcc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gsrmidaeu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gygiowldj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gbgakffin.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gwunhmhea.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/ghfzibuvc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gnelxodfy.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gpnoaulpy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/geqgbwwwh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/guvvrdose.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gaigleysm.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjkghzkpo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gmawcdfuc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gvympbzwl.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/grflzqirj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkefnkalv.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gujbvwhnf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxgkbohyz.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gzqhsawcb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gzsubnsmx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gwudweqvd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/golzeryzj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gjzgmlbym.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmsasefgk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gnnafwcse.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gzpnmxehf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmxwmafqj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gejupqkas.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnilwoitw.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gflwveayv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gnrsbfczo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gfkkskgjw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbeogrxgi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbzeusric.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/ggyhsewhb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gsfimtiqw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmawgzcdw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gyuskrxiv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaowxhocd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gstjhkgtp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gcilbrvus.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghhydndec.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/glovnlrgr.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gohohljcc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gispqdqwn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/givgtpugr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gxexazyzj.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gdakfgdca.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gfdhaojma.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gukklwvie.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gpjahfhdp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/grjfbybgh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnklkhiku.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gcaspmnfj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guyjcicvv.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/ghptonqkh.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gqxrulbmp.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gvsamhprk.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gghzzanmp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gksbebkdu.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gbmufphxx.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gwyrqbolf.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gfvmgcage.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/grqawsklp.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gfumvfseb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/ghaksqwhr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gttntybei.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvualttdu.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/geqvzcymg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gxlkahffs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/giwgiyxwz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gsklpkmae.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gravaaaoo.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/govggdyex.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/godwqfeaf.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gryzvkmxi.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/guzwiwwlm.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/ghivrblqb.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/ghbdjiumo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gifqptshq.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gajlbqack.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gdukenscg.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gwyipccia.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gsgbzdisp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gffkjacgq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gcsvnebsz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gupokrreu.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/ginzqfvrh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gqkfrclzg.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gkrygoads.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gcgdswjwn.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gzxevlgda.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gkzhizduy.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/goaslqwnk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gwqhbejrm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gwsxuyixk.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gfrktoofm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gesxxojvl.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gpjuzisci.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gdkboexga.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gseawqcyx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gwbxpupvr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gygazszdl.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gcfjkmhdy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gtpexpbax.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gkuuaivsi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gdottkzkm.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gjvsezkow.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/guviawisx.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gkjibmxrk.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gbildbhxo.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/grtothflj.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gknbmxhkz.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gjrmiwrqu.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gmamedhkr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gtxeipckq.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gtymluqxj.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gcjxxizxh.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gusnzqxax.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gkzcwzqnb.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gbmylfzrc.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gbfeuufcd.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gyashokwe.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gqmzwgncx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gzhjdvxcv.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/ginfylqxt.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gmkypuqih.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/grebacglk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/grffpbqah.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gvfpwypvb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gxodtcmtv.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gttlofsoz.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gdbfwyjgc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gkzfuzobn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/giecquvoo.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gvshsozph.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gayxljcjv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gcdxngmfj.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gscemdwli.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gkkbxtfen.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gijycrnyf.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gnykcowrl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gexyusyxp.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gukrpotmt.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gbayenbpx.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/giilcavhi.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gylvbztgb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gqlihfzny.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/ghwkjtuxa.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gmytdttbd.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjewbexxj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gezeprqjy.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gjpedyrnu.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gfohnyeew.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gmgizevie.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gxcshfohq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gsafcekvc.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gkotairnd.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gzfbdfvgp.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gtyvwxvpd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gqkomosxv.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gsqtbrfht.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/grhnrubfh.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gfftqyvhw.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gngytlvah.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gjxmupsoo.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gkofxfuuc.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gpyukujph.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjljnyihc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/ghzurtnon.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gfogscnkd.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gzqayvbwj.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gcvxiveep.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/ggjmtwibv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gmdrobpan.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gmgurgtuc.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gzrczqpnp.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gnzpsugbs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/glaoijqci.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gxueasxmj.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/goiihcdvl.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gzvgwafwh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/giqlhiuol.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gsebpmwql.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gnqvzoivi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gpcoimakg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gltorgbvo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gdrtkoami.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gcheftuqk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gjaxpiwjc.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gcrzhibsy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gjgkvhlrj.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gqvzmqbfa.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gzqfdzmry.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gwjtamgzm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gajkaaaon.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/glsmlypiu.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/girokohmz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gsvxustch.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjewvfdwb.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gjkfmrsex.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghtvtsceu.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gcbzadxan.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gjuqmasdp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gfzcffzgo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gchmgnogf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gyhmvcoec.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gtgcmtpmq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gzfwbwsqi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gsjsyvvmw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gqhqaxxxh.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gjqratzen.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/goddnlvow.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gfntkaadv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gghfueypx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggidmuvon.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gbimilvxv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gzcsaqbnb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gebqcqctz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/grjktpadu.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/grtfbfwsq.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gbagzgfii.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gphbzayvy.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ggihzmhqt.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gixfznxwp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gvavixtdq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/grijyeivo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gtttadhkk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gcwlbofoc.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gmkjrtbnu.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gtpvykxwi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gsaxxxjbw.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gwdbjirfg.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gthnelqao.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/goqnqfpnp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gilbaxoct.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gvfnatmkz.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gqdudirpp.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gedadwoiz.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/ggpshtwzl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gamktmtvl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjscrnrud.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gtmoerngj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/goirrxtjl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gzndtkxnf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gepzkcevd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gzzwghjky.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gqcecahnq.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gpxgznjyc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gdxkbwroa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gxwftgqnu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gueoxkbvj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/guvinakwm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/glnbkmylt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gxvbasvrc.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/ghlwxztim.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gqhbftoqx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gwatiwmiv.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gsuomkudj.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gpruktpqw.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gejgcgauz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gbynpuxtb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gbcpzfjsu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/ghnadguaw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gspqhmltq.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/ghyxzptxs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gabtwwgzc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gxenagyfj.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gqplsluex.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gylomaqzc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gfcbqyjxo.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/ghxtrgyno.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gawqmplah.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/ghermnjhs.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gfovkathc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gcmitwndw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gqepabbly.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gtbylbcaw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gdidfobie.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxvcpjmi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gcndzjktv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gumnjrkgc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/ghihgreyj.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gihwlajkx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gfjvgffal.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gcdqpldxf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/grlpaoicu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gjejbnkgx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gkscbkkbv.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/genvrdxyg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/ggueldjtz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/grviddhiu.sHtML


<!-- 参考信息 -->