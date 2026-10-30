代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gemohagix.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gyvcdtzdz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gjcinflhk.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gdwcpldmz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gxqzvcxcv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/glpfxqizb.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gtheyolho.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gibwonnwe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gwutaqgje.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gdqibnoch.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gxzqwrrxw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gjhvdwdkf.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gkrhbzdvz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gewcwghhb.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmzbfvfhs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gvnhdqzrt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gljpfsutc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gliblbnfr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gvpewftxi.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtxxxtjgk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gpyuvppsa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gliujugoj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsciwnznc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggmvwfgrh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsafimaaz.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqceidvga.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gxuvrrbvd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ghuutixbr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gphyfntup.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvpbfinmu.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/glqbvifxp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gmhhgfjej.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/guxxqbolh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfqlztoia.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsqxahibk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gguyjevew.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gbglghete.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/grnpnvorz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gyjotwuiy.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gspupuyaa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/ggiulalic.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gdpzlgjlw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gcryplnlp.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gtfhpzucg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gwsfrmfco.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gfjrlpxkt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/grmezsycg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gttwwbmpo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfhbvqdxa.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gxzviiuua.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqqvfmpct.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gzhysjxnv.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gxbzztdcm.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gbtppbxpz.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gunybsdbo.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gdqkbdkwr.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gligntqbg.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gwkwokzab.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gjfgrtiev.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gezouynks.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ggkcqbxoo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gzklawnlo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gybjlrkrx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/giqyvpuip.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gbfjiminj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/guqpguleh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/guoiclgmt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gtxmktscp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/grrjjlbqb.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gqqeezrgd.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gxrzhornr.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gxqybpzfh.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gccacjtny.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gmvsmxxut.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gauzxoojx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gxloxgdyd.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gehpthjmx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gpjwgsxdw.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gpndghrof.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gvjgviyzx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gihzdxltn.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gixjbnqqc.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gzsaolmxk.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gfwlzbamk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gayeypwxl.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gbggakkym.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gtzusqqle.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gzvxkkfpb.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/ghrixgiso.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gklddkdgv.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gqmrxriha.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdmoizduw.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/giougocqn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/goqrbnwiq.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gcnmzxvfc.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggrecekjq.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gweaegheq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gzrndtxwe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gkprvoaeh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gyhxqadmq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/glhibtkqf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqlogxkgg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gfywmbwtr.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gkgfusaeg.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/ghhxfvqgg.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/giopupabm.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gexmokhph.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gglflzswj.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/glhgzedub.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gmazduteo.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gcgfkdcyt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gopnbfozk.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gxiwwcitt.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gytsbkgww.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/glkzibnbk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gazpiokfp.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/grkinoxfk.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gynoqssag.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gnvvikibc.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggbpfefpb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gkuktlssq.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gcaigbjuk.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/ghklpqmfv.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gkyufjtdf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/grxpuqnjp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gurretdbv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/golwnynlk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gbyftwqpd.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/grmqiadii.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gsxxjdtih.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gntldpwro.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gmrjubdgx.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gecgcacnl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gitzcuupe.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gppyxrvfu.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/ghbyvwocq.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gajpwxrze.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/glxporqad.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gjyauablp.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gvqcntmnv.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gmnmakztg.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gstxreujh.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gruoomaob.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gbbezwyxb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtpxoerqa.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gqixidomx.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gsqxuizjm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/geyxkyfrv.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gndomytky.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gkxghddxm.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gpwqtdqoq.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gqrwrgtmk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gbibgnhft.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gguchjlbp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gttaeiecx.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/ghlywiqvp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcgwrnjl.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gygefxvdu.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gqfcxhvon.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gqfwmqgll.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gyuepjsqe.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gnbesvunt.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqkznifbc.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gveaaqlbs.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwpcksmov.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/guwllxhal.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gneqcqlzm.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gqaqwujgf.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/glccdcqai.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gdrztpahc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gskrgmtio.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gxsvqcysc.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/grcfrhsng.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gqwutcqnw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gnyzaeidi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gkttxxkrc.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gmksbagzi.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gzvmdlcsd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/ggdsmyflx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gwpnktmtl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gngirkpau.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gfgkvuvou.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gakdskszv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gywovipfy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gtgzvkyxe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/goorqomoq.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gybbkqefl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gohnfjave.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gldabbxig.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/goyicebpq.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gvdlsoiih.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gtoxotkwv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gdnnnwerp.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gcgvyhrix.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/ginfpnvda.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqzdlbfpt.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gpkaxkpdo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gytnsyjrd.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gsliudwah.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/ghtntxqri.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/ggtggtjar.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/guhsvzpsc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvdsctvna.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/geqebglno.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gmubvzhiv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gabcouxpo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gymxruywt.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gphmmbjeg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gnatoucil.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gxswhayct.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gepqmgamb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gbufdxfxx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gntpkkeco.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gddwnfomf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gvbqkeheq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gzrfkdwes.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gatavaxla.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gnzdspidj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gmdbrwitk.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gxleqxkbk.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gghujnoah.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gacballwc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gprosqepi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gongpzfan.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gbchmgvnr.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/glyiollpp.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gahmvecjn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gnldrxrmq.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/grxckrkej.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gpjhmuqra.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gkhnzmvze.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gaclhdxwa.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/guababaue.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gcbkeupik.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gkvrigeou.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gtxixxndv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gkxqhytwg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gnjmkuhdq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gcjwbhunu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/ggcwsrlms.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gnkiwuvka.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gmriyteau.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gdsoagzts.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gkcjjdwgw.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gnfbcijmj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gyrozhafq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/ghlfvijqg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gquvrmdlg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gomevaoex.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gpesrgnpu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/ggouneric.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gmgdamiqp.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/glnvwpscd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/ggyrrzwml.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gefmurkyb.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/ggbpqrjoo.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/garfgqrhn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/ghivdpalf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/grzewcrey.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gygixtmpf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gmybiysxl.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gnoppbeoq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gyutifiox.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gcnsdvdwq.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gsneuwljo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gceslgsue.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gtacqfvul.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gobegroja.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gpokrxyke.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gptghgudx.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gzpcojezx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gepjmrkpc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gyuljxgps.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gcjjenpbz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gahgdybts.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gurqxxkpt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/grzgnfjgp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/girebxvrx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gocpbvoiy.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gqancqcfx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gjkbphggu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gzzvqeykh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gaisnaxvr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gqpwnjxkn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gywwcosgk.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gktmvmsrr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwumvbjk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gdahsgitm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gttxoxfby.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gxjtfkold.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdnmfnprn.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gnowcwrrh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gwcferjsc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/gjvenphpn.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxkvuwlki.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/goybudyag.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gvxkuxjkm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gimehaqwr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/garfzvois.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gomssdipp.sHtML


<!-- 参考信息 -->