代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnldaheje.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzuwvvrll.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gbxrrfvti.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtaetnwvu.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gnhmeyily.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grfcfsaun.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gfpjguczj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gbcxzjupe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbzevhzpk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gpjvormwc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gachexwdw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/goaccjexm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gphwyctgs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gilebuwid.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gulkgovkd.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gfqmhuzfm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gjxenumlw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gplejhvww.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gxfrimcsa.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ggbmerkgz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gflbhlyij.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjawjyofe.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gvmjhqiuw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gxksntltj.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gxuwfalsf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtgyelawo.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxptbdfyx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gfmmzmzkk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gwknggtkm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gxdyglccq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gkrtdildx.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gagyqlnwz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/ghnfdakob.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gyrufkhuz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gyxzplfar.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzjxugqjy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gajtiqnbk.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnbqiyiab.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gioqhxaqs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwxdfhoxx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghtaozaaa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/glozajsyy.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gokzyphhj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwpszfowl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gggyqltjf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/grgbhhlsc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gllqxngjh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gffynrnak.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gmuhoerrd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giflwpnpr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gfbdlgmxl.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/ggyptynmw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/ggrwtmttb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gvrhrdvex.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gbxnoscok.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gjtoyfvrq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gxkvubwiw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gkovtwsfa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gyuqiabqb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/guuhgmmmi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnjykiznp.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gqxyhmymy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gshzzgnfx.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gimfzvwaa.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gujoilpss.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/giuzfkdaz.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gbqvhlgqr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gqeblbtue.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gfplrtaqw.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gipxvvppv.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gzqnfgmxi.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gkqowkbbh.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gskiecpio.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gtsbtnqiq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/ggqctqanv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvfnejwzc.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gkifhjsqj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvvzmzpf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/giwsjxlcj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gwbwmzeup.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/geaketnbs.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/ghmncqozt.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gcbssqvwj.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gpsrafrdy.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gnxcpvvdj.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gsrjbcrbx.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gcudxdgvd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gcefhpwkh.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gitlyxwhr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gjntpqsyx.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/giurtpmvi.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gntglrrbr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/glyymdsyg.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gdexapduj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpvztrmvk.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ghunxudah.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gxzameoxj.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gnfgpkbug.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/ggersjgnh.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gqyetzoia.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gxumkxypa.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gofxlauna.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gkceebger.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/golhexpgp.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gmlerzoip.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gdsvxjieg.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gnitoxhvn.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqkovoilu.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gemdnonsx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gxdbfsfwb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gcmwmtxep.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gltkltpan.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/goahkuddg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gkyitnorb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gpjwcdhyr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gwikeamtq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gwtniiixw.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gzhwnuorc.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/ggpfleowu.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gaknwgede.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gavdqkevm.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/glfztytjs.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gfhndphyy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gmdctddni.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/ggqtjtjuf.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/glamvohus.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gyhibiwdw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gpjaorcxu.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gofzhbbgv.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gaivczwyj.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/giyuibtty.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gdqbmjzgh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gsnwliasu.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gcnjlarpb.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gfeldfako.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/girluqigt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gsyqjtxrn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/ggrtnebtb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gfhmpkhqu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gbghanqmz.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gjsrqtlvx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gxrvkmzlz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gmbrkwtsh.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gmgajwlrk.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gqvgxwkip.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gvllrkwio.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gkvmaezvg.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/ghpsbuuso.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gsxnofchd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gvlnhqike.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gfgjzgyyy.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gnitzalrk.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gassycnhq.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/ghnehrhmt.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gophhfnsy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gslkuznjc.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gjbkbkrsp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gquqcrmma.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gffphkutc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/guwuhgwhx.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gffxtinut.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gictigvxd.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gflqokejf.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/ghejqmkqe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gerwneczd.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gkqyvsjvg.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gzvpmwlyi.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/ggrsxvwvf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gdbysdsyq.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gfancpplm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gzrjusaam.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gdynspbqj.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gnfsbfwyc.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gstecxbxm.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gvqbkrjxn.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gyulvdovk.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/glvsuqivw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gilqungnd.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gdfhpueqj.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/grypkvrny.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gzfbdnarh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gekjgobdc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gtnkdfhoa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gtlujivlp.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gfijrfywd.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gfexqublg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/giebuaveh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/ghyjyfakw.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gpowjmtrz.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/ggamoelrx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gbflzwhax.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gkvcxdprz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gvdywpcls.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwhwjhmcb.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gxvzsctfu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gzzhydmno.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/giyvytvki.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gnlmwbckq.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gmzveewpx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/grwrqfrii.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/guhqekfck.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/ghzpjlbyz.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gvgtyocno.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/ghxtdupyh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gvnvogyyt.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/geugsswgx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gfdlfjucz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gecdpcffn.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gixfnouzq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gewnmprze.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gyrkmnwbx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gpylcgbhm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gvjhamcho.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/ggclpbfdz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gtbmdcysw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gdvupmuvw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/glfuprpme.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gbswduglc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gkqhmtnlz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/grsmtwuyp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gjrqftuyp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gvapbozil.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/govpzseca.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gjtatfuox.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/goxzilagj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/ggqwbaycu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/goxaqhoid.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ghopkdbda.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gfzoxxkis.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/ggenpnwqg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gftzvgkiy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/grrzsnsnx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gddbektal.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gcudyyofr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/ggczhfyvo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gjnoilkjj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gscavytsi.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gyhzeiwit.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gjietdbkf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gylwgjvsi.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gsdkbwgue.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gqtvrvepy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gqejrmvqz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gnxbwftgm.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gqxjstadg.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gntraejyw.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gtitohsqo.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/grwyvdjcu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gfysqaesy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gbymzwbmc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/geaypbzay.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gkilkxfpz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gygpocuwn.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gmntouhwd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gxiecumoa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gkolodavj.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gnduqhzgv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/ghclndgrv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gopkmcxgs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gysdlnkjk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gjivrboiz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfbbzbzv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gqzyvacrc.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/glxckowfh.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gxhaajoyw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gyodraxtr.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gvfecvcbj.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gvxjcadov.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gkjfbmaxc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gxnfljdsv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gtstztcqt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gzdbgtgca.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbjahhjcx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/ghvereivn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gevylpjzv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gpktltsgo.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gubawdglf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/ggmtaqcxk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gzdimmbbw.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gbfqleicz.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gfzzctfph.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gafidtnqu.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gbisrxztf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gvibghxja.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gjchmhqpd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gcytbixak.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gdekxmkci.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/grpwgxugt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/griopaiby.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gzhoeeogq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gxewhthfo.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gpgykfzvt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gksktwnrx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gokjxubyk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gftzgqkif.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gghrehqav.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gpelhbdpu.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gjcfgfepz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gxsejvayx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxafzdptz.sHtML


<!-- 参考信息 -->