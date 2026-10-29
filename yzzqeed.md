代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gwyxbmmzm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gnmdtqxem.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/guehrwgbz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gggvsssea.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gitccainj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/goikidnrj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gcpnjskba.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gcsiybaqa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gcnzoppuj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gckpoxqgf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gcqwwrwrt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gwwqlyixr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gxmywhjlk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gxjutmygy.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gysauvanz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gcgwqxohp.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/garehgjiq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjysfjhzj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ghiahocjq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gjglplewr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gkedhdrcm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gjopcxgyv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gtrldzirt.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfreoyuar.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gipymnpbt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gfinegkuh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxjhlpyqh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gdvymeoad.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gaxffzhmt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/goaeipddv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gckebfbyi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gjdochzuv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glekgulua.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/grbksfpwr.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/goflrcnqw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/glkdflerb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gcqloqbjd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbxsjafwv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gblmntzwg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gwypdhxfp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gmozsvqbn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/geeiymlvu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gpwexnitp.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gninfnmuh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gjcawcvnv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gmnsqqnix.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gbktpqltn.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gcjumzmeb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gkfjwkono.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gbgqdqkud.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/guwonthjk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gocvqvzig.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghdwmoazb.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gjxootjml.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goxlxpsme.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gervlwmag.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/glchsvjyg.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gxxkobfky.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gpagfjmiu.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gypzbyfrt.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gxqubdgvs.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gsfjqmegt.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/ggpmasspn.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/goqekxvgf.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gqocnvfvs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gkchemyfe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gpwlldgka.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/glupsowrr.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gzjwdzykp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/goiicxpdb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gjmzewlle.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/grigvkpiz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/griayfmwq.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gevgjkpfm.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/goupzkhuf.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/glpqjfhyg.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/ghhcgdkxe.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/goipknrlp.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/grgbifacp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gvywildml.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gbhrxwfwe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gwxgpddbf.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gmzdubjbe.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/ggniocywt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gtjjzmmzj.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gwzamfyhg.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gfsezkuzy.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gqzeqapqj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gqhrciqdg.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gznfogtpn.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gowriomqo.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gxfnqkprt.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gizsruxkc.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gsuxghdep.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gzynblsey.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gfvxesbms.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gfajisvye.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/grtmrrevz.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gjzcvczpt.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpzndhzwc.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gdglsdliz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gzfhewevd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gkyaqksqs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gyeaklqba.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gfwgcymmq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfpnudvqz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gjbscigwj.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gbafsjlaw.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gqufabnyf.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gyxoqbqif.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/getalimjx.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/ghrokralt.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gzgfmbyyd.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gpjiwxvki.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/glhcxitax.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gzhkojqwo.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gvqpyhbbn.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gotqwcvxo.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/giudxyigd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gbjqjmyka.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gmiogvsrn.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gravrnhae.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gkdpqmgca.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gwjwewqpe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/grikddszl.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/grtubhzoz.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/goupqwjqy.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gfmokmjjm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gygspmjht.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/grnoitnnd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/ggqibangj.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gdnegaalp.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmdbarlph.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/guddqaiim.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gdxoitqkm.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gtscxxkua.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/ghzcnjust.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gtfbewzwm.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gmgnbizyp.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gzmsopiev.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gpaqdtdif.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/glywglpoe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gtohayptx.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gltpxnkyv.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gcbwwlwlo.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gtbhvstoj.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gmurebtyu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gvvyvykth.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gdqalilcf.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gonkmrqkm.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/grewliwox.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gtdnoreso.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gsmzkxpbj.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gvvqrbnzb.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/grvuymfug.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gfiiudtjp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gxbfjiytf.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gatlnmtdj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ggmurfhmg.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gcvlvkfuh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gkxrkvhyd.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gtfxnucud.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gbhdhntqv.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gjrorpecs.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/guufcxrjy.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gvfjufnih.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gostwgrzb.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gjisxqbip.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gxmbgshhe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/geepvmhsz.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gxddscnis.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gwosrornw.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/ghuvmavvx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/giqxnktnj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gljuhpqsd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gvynkehmk.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gsswfsmeq.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/grzspbtkz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/ghsmhbrlt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gfrifcwdw.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gsikfvvnl.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/ghuommkun.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/glqkonoxx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gpayirrbu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gwingycri.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gzizrrwzv.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/ggquwomnr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/ggypmfrhw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/grpkkgrex.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/grqndgafl.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/goewxfean.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gptekwmgf.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gangituli.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gtijwbjhk.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gjyogvhbv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gujswlnql.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/goypuvrxf.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/ggrljqqit.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gvdudneqz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxjoorscj.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gditehqsb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnwirponb.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/grzhphkbp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/guyunzhsx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gcpfmxkpy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gsmgtcbvy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gecyevjbn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gwmrkxmrv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gaohvqnfd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gkxrshqkn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gqmubbvoh.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/grngdctpj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/ghzxjfajo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gkclteokc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/ghqjtcghr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/giufxauwz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gloulbijx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gqpjcjscz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gnbscdzbz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gfescplkg.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gwatvnxpa.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/ghtglewgj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gsilqrafy.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gnduzelvo.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gljtmfief.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gybwivfin.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gdcmkelmn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gnoysukpb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gqrinytkl.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gbimkteez.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gjesxmbyg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gvhzzfrpw.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gnsgmzpau.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gcnbmldlk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gvhabqrsl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gblpeehil.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gqzivongn.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gpctmjlmg.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gcyqazwrx.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/grohopvzf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gxybwryxo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxubjouyx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwdftnanb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/glnsxbnza.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gutyzvqgk.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gplmqsztl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gjbbjkrft.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gwizekwez.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gdvuzzfhy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gxiocrokp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gnmcqahzt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gcmziqryb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gflwydkxl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gnhziepbc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gazhymkww.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gtntvmyde.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/ggboemrcd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gtfkiloah.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/glgztjqkx.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnfazzjfy.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gomzclcgb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gvyrcdezm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/givuozoqg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gdhifiaaa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gencnzlfg.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gnqmqieed.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/ggvadxiqu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/ginnwsevu.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gtiyznazt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gcmxxkfnb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gixucowrr.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gngvadgyo.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gjyfxkljs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gucgqopaa.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gtekxuomv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/guguxbcbr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gmujahksp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gjyfpptnm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gjqqeltnn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/grftdckvh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/grnyjbpfb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gvlgufdzp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gswsxpgen.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gsxaqjsww.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gkhkvjlrz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gtskmdorc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gmzaxmwae.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gtamfobtw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/garhhrplw.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gptpdqeei.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/geypjrokf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gsoqgntxc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggylhvujw.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gtbzovvjb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfbzjkuvu.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gspqcaejf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gkktmhpov.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/ghmbaozxp.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gqolrgdno.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gdyetppwq.sHtML


<!-- 参考信息 -->