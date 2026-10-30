代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fanxiaobao.xyz/Article/details/gpenakaoc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxhpbmcz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gsffytftk.sHtML

[F08] 遍历目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvabtnmmi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwchzkbq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdczzuyic.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gnzcnbgbj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbputeeu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gmagdelpx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/guomtysci.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gmbkmtsqf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gnjhgedgz.sHtML

[F09] 获取文件大小
来源：http://m.share.fanxiaobao.xyz/Article/details/gzljocrvw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/ggcyqdcvu.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiiwtyxo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqouztjf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtiqyyjf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnyupain.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fanxiaobao.xyz/Article/details/ghnmznezq.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gpjdvnceo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqmrnpkr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fanxiaobao.xyz/Article/details/gmnnekgzk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/grpodimxi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/glbapxtqn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gfrzrewmx.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/grtlocubw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groklpsxq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzmqlrlo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxbzetfo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmekrhay.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavulrpfw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqnzjdgz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gezwciexs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjszoqmao.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gpdwuizas.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvsfxrad.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fanxiaobao.xyz/Article/details/gltkrtuwo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfbjtqcv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gydarteeh.sHtML

[F12] CSV 读写
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxdhqiib.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fanxiaobao.xyz/Article/details/galbdcsbc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fanxiaobao.xyz/Article/details/gmcefrzbf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvkhjbct.sHtML

TS:   // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gprrfcdze.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtqbgaiu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fanxiaobao.xyz/Article/details/gjvxgjrul.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsidatnud.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gepybvlmo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geaqoyfxt.sHtML

G. 面向对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpfrbhyw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtywviuji.sHtML

[G01] 定义类
来源：http://baike.fanxiaobao.xyz/Article/details/gouskerhj.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdjxizrk.sHtML

PHP:  class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gilaieqxe.sHtML

JS:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxkqkflgh.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fanxiaobao.xyz/Article/details/grhhydbyv.sHtML

Java: class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcakwqidc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznccmfuh.sHtML

Ruby: class User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfevrjqmf.sHtML

C#:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gaptjfmim.sHtML

[G02] 构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfksrhojm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwxeoqib.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjucxgdjz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gifsakfta.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gplstcrqs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiapbbjb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gumvkacjb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gtzjraszi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsgukmvlt.sHtML

[G03] 实例属性
来源：http://3g.fanxiaobao.xyz/Article/details/gnbnhglvt.sHtML

Py:   self.name = "x"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvtutlib.sHtML

PHP:  public string $name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/glhnfcfzd.sHtML

JS:   this.name = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimvdcjhv.sHtML

TS:   name: string = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzitgftml.sHtML

Java: private String name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgenurwj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkixdlosr.sHtML

Ruby: @name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gslvovfmv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gsbpwujsc.sHtML

[G04] 定义方法
来源：http://wap.fanxiaobao.xyz/Article/details/gflvuovqd.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/ggnmdgerf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzwnxvsi.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaqkdtrn.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzuyfwzug.sHtML

Java: String greet() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gltbogldw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gunprfkyb.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsjzcbbn.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/grsmmopyt.sHtML

[G05] 继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gbedwopnd.sHtML

Py:   class Admin(User): pass
来源：http://baike.fanxiaobao.xyz/Article/details/geaopliai.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gipkdgqhp.sHtML

JS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gkzzkhufd.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpyjecex.sHtML

Java: class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbcouhma.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gricluolg.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzrmuaeg.sHtML

C#:   class Admin : User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grazznngv.sHtML

[G06] 重写方法
来源：http://wap.fanxiaobao.xyz/Article/details/gwenutmhy.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvjinckr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gysdzlytb.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjxggzcu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzickbvpr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmdixybgn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fanxiaobao.xyz/Article/details/ghkqslsga.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fanxiaobao.xyz/Article/details/gxuufywah.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdukxcivi.sHtML

[G07] 调用父类方法
来源：http://baike.fanxiaobao.xyz/Article/details/gswxthrhf.sHtML

Py:   super().greet()
来源：http://wap.fanxiaobao.xyz/Article/details/gvotzmcnv.sHtML

PHP:  parent::greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdboslff.sHtML

JS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkapyvbt.sHtML

TS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyefpjwcd.sHtML

Java: super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuowoixj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gtazyvqau.sHtML

Ruby: super
来源：http://m.share.fanxiaobao.xyz/Article/details/gwttpqnqk.sHtML

C#:   base.Greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqzufbye.sHtML

[G08] 静态方法与属性
来源：http://baike.fanxiaobao.xyz/Article/details/glbgmdsal.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fanxiaobao.xyz/Article/details/ghkbtgcrp.sHtML

PHP:  public static function f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtwjlicdj.sHtML

JS:   static f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/grfhvuooh.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdmfbdoh.sHtML

Java: static void f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwiczxznd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gculrtmmq.sHtML

Ruby: def self.f; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnqnbzqj.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrhrplwl.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fanxiaobao.xyz/Article/details/glgxyxnct.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfixqgije.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fanxiaobao.xyz/Article/details/gamslteyc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxpadsyh.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdidpnueg.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbmyfsfye.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgcukxcf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gfswartzs.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsemzarf.sHtML

[G10] 访问控制
来源：http://blog.fanxiaobao.xyz/Article/details/gwtjdfdra.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcfhoffl.sHtML

PHP:  public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/grhinosmq.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjmjmmrw.sHtML

TS:   public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtvgaute.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fanxiaobao.xyz/Article/details/gmprbfdqo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjirpfazs.sHtML

Ruby: public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvbqobgc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fanxiaobao.xyz/Article/details/gcazikjli.sHtML

[G11] getter / setter
来源：http://baike.fanxiaobao.xyz/Article/details/gvsqspqyl.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmpapfgj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfpswzvij.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geteevnqy.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlqhbytr.sHtML

Java: public String getName() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtjrozalb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnbjzkpa.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhkfeoru.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjsuansr.sHtML

[G12] 对象转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrpohfpu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrtgdqke.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdkgtigl.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gojwuvknw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/girkyqnui.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkmdiwbme.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/givipeygw.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gkjbixfag.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/genekgrkq.sHtML

[G13] 判断对象类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhvnycwp.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbckymrs.sHtML

PHP:  $u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/ggabxrkst.sHtML

JS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gppvwuerd.sHtML

TS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdgzpkay.sHtML

Java: u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gokfsgode.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfacutsf.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseciwxbb.sHtML

C#:   u is User
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaxiuepj.sHtML

[G14] 数据类 / record
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfgvnont.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fanxiaobao.xyz/Article/details/glchacqqi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/gahmbzixm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fanxiaobao.xyz/Article/details/goeanyaqr.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fanxiaobao.xyz/Article/details/gqxnkyoqb.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsawpgncj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgcqyhqa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbwqfjey.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvtnekeg.sHtML

[G15] 枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrmffsxp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gsagzcjax.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzsuqwxpu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fanxiaobao.xyz/Article/details/gahpdysae.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzdbncsj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopdxqlzr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadbkhctx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fanxiaobao.xyz/Article/details/gdbtncgsb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/grjwsmgtz.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvxzpgin.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fanxiaobao.xyz/Article/details/gnrjbseie.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fanxiaobao.xyz/Article/details/gaxobdbbd.sHtML

JS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gbozlsmop.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuitvmwh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gsarkncgn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gaprbwgmz.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fanxiaobao.xyz/Article/details/gobxtjcef.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuswgodi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzkjbbbip.sHtML

H. 异常与错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gglfctjqm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkbzugwk.sHtML

[H01] try / catch 基础
来源：http://mobile.fanxiaobao.xyz/Article/details/giyerqwgf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fanxiaobao.xyz/Article/details/gzlzkrwrg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmqzoxqo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmonmrlrs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlzwmhyj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjahbsflw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glukhvjil.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fanxiaobao.xyz/Article/details/ganfvasdu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fanxiaobao.xyz/Article/details/gatlboqlq.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fanxiaobao.xyz/Article/details/grsdrjrcn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fanxiaobao.xyz/Article/details/gajvueqvz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjisbljbr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/ghfoieqbt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhwlyfmr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpzpcbxb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fanxiaobao.xyz/Article/details/gooyaksvq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixewwkur.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggdqqgduh.sHtML

[H03] 主动抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gywwvhntx.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpxlsudm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/guhgrmkiw.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gcjdhixke.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/guvfvgkel.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gklvptbaf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giymsuiie.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtfycnfr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gkczdwhbh.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtycftskc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebfjimrr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxwqaoey.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gssjfmkkm.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrtjfdll.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsebudvnm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitskqxbn.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gytipznvj.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gscdbacql.sHtML

[H05] 捕获特定类型
来源：http://blog.fanxiaobao.xyz/Article/details/gbndeurwz.sHtML

Py:   except ValueError as e:
来源：http://wap.fanxiaobao.xyz/Article/details/gbfaczxkr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fanxiaobao.xyz/Article/details/gcfpnsced.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjknmljnq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvtfcziw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnocnwrgc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcfseyez.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geobkqecg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyknxyro.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcpqvutq.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fanxiaobao.xyz/Article/details/gokxkzgrp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gpgsugszw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gndufcvbt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gmfmdfxuh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fanxiaobao.xyz/Article/details/gxthjzcdq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fanxiaobao.xyz/Article/details/geatagdzq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gidhscwso.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/grefbxaju.sHtML

[H07] 断言
来源：http://blog.fanxiaobao.xyz/Article/details/gusfpbnmw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyvbolpw.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoounxhf.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyjmjvua.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcyfkhzf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlguggna.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvchtwxs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fanxiaobao.xyz/Article/details/gxcvhlvnq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjbmgvpt.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fanxiaobao.xyz/Article/details/grzwrnphs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fanxiaobao.xyz/Article/details/gqcrhikbf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgdlrzgr.sHtML

JS:   e.message;  e.stack
来源：http://3g.fanxiaobao.xyz/Article/details/glkzcxubu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyowbwzgm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsphaatw.sHtML

Go:   err.Error()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgswaiwc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfoacufe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fanxiaobao.xyz/Article/details/gigcsbtpm.sHtML

[H09] 带错误码的异常
来源：http://read.share.fanxiaobao.xyz/Article/details/guwufhqiu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwbimpap.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/geomkcajl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fanxiaobao.xyz/Article/details/gidxjyssu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlwjogvo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjavgcgf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaignrvw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/glfkdbisw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gatqpxvqh.sHtML

[H10] 资源自动释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzhqjhvp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gustltgso.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fanxiaobao.xyz/Article/details/guwkvbfxa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/gkxmiskgu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fanxiaobao.xyz/Article/details/gyercnmml.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fanxiaobao.xyz/Article/details/gobrmplln.sHtML

Go:   defer f.Close()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdzxxwnn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlgnbhzm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpdahhfe.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzkffefo.sHtML

I. 正则表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gqltbxath.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfzngzxmc.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqchtnywx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrkwfndr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/ggebgyjzz.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsynyioo.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjhdehbu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fanxiaobao.xyz/Article/details/gcrwtpbiz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fanxiaobao.xyz/Article/details/guscycvtl.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/grytaptuu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gofwjrrnz.sHtML


<!-- 参考信息 -->