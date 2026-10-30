代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxrudhtpf.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gmgkzreog.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gipbftnrc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gygffugnj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/ghclulfza.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gnsjrerdr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/geoxmshif.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gpyuunibw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gujntlope.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gdhlzpipw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gwyhhgpnk.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gmcwrbamw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gymawhoxb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gscahhbaf.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gjsaevsnv.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/govetisjs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gnmjvhzvi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gwluwgpgz.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ggdpuycjv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gtzagmtpo.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gmhzyuzkz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyroscbae.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdhwgcuac.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gumytevll.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gzgrzkcbc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gzdykggih.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gcxdbhpkz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grbfrohqw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gfzgiqthd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gvigppywh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gknxwsqcl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gusozagqb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtnxdcddk.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxiavogld.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/ghjemnsvo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvfntorqh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/giyziaytz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gskqujgoz.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gcszuuias.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gkcubzaio.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gxlcyvggn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcigeteio.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gjhceapio.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gnyizteov.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gdctqpvqn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvciycsgw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gryvysyla.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gnmhmtigi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gdvcqoymp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gmswliwpz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gvcmdigyw.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/grjjiprty.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gkjcuxpdq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gnhusnidx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gpiizoume.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gaoalexjt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxahxjivv.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gvfjbgpum.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glzcmqzwc.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gplrgrrwn.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gpvovmrnj.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gqvgelfeh.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/guamioypo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gjbvittfk.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/ggqwugwmc.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gzlmamwif.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gocficgse.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gsrxzrtix.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gbenjpuze.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/ggsgxrjaa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gexnuhbkn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gyzjfwnkr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gesbeomga.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/guyviiqzy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gootxkmtl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gzanaadbd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gsraowqli.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gapvwjhve.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gxcaxferp.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/guyxvmskz.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gngwddxov.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gdwregfwh.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gowktfywf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gsiuboyoo.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gndufhjcb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gugsnfnmh.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gxnhbtztl.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/ghavkuess.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gvkqkdrrh.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gktmcylyl.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gjveffmbj.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/giduycedn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gbfnobqzf.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/glijxaszk.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gkdaawlvi.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gtpxpmfuk.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/ggksvpeyx.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gcxpueizl.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gvjqztuyu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gkwfauqxo.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gxagzuqrg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gubrfjiut.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gjdfiwzko.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/giufahuyp.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gdgjrbdbe.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gsbafejuv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gblukikwa.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/geynjbfqd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gjalwxwoh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvgepzgyz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/ggskuayhe.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/guxdinata.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gtljkcome.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gnhknyvmt.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gkfumhheg.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gyplahkpa.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gilmesdbq.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gmmopaoaf.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gwuxuwkmr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gtedqjhsy.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/geejcxsnr.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gftppqznr.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/glfpuvyzf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gfrdmcwxu.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/ghzerrgbb.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gizkevyzb.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gorsavcre.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gqjnnusqt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/goklvrimm.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/ghrghxocb.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gbzclheqg.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/glnkctfxz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gmfbrbudc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gplxnwdts.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gbpnmhsoe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gcnxhkrej.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gakmjmyot.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/glfctoncn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gbgtlbftt.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gvfgnvpkj.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/ghwnolqci.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/grvaopqrc.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gbjobplmj.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gaotexxbs.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gaqxbvhtr.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/ggljmzmjz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/ghisylizq.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gkoowokua.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gkvrwhism.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gbevyvwec.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gptekpnzx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gidpxrwfv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gammhmuoh.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gynmtenlp.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gmfzvysce.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gwxxlvblm.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gzbszwzyv.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gqworvfrk.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gqogygetc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/ghqrikppl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gscaspdvu.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gncftdgsl.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gnrfwjebg.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gjztbjraq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ghjbnkfdy.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gqxgugvjz.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/ghyvohyvx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnjsxtysu.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gzditatqq.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gklialdls.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gzfxjmugb.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/givhwqmed.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gykdytaik.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gkqazwnpf.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gqrlodopy.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gqnqzstpc.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gsivitatp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gvhhscbqs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gttuxtulq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gtqeisasi.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gxpffwvms.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gienpgrwd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gfeqwdgyr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gfkbptuos.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gpwpvopgs.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gjjxnxpva.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gdxzixnwh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gefficlyf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gtjbneikc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gjiyuzwgf.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gpyyxfesb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/grjewhmjw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gxanbquii.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gzumigbxx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gxagtginm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/ghdjxdugj.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gpsidewor.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gpsfyjxjc.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/ghnheshoh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gkecssntn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gdtphyxbd.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gfoprqsfb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gqzrtbdww.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmvkulcft.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gvqxauvsl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyjdtqaqr.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gqzytnkwd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gvyzuawuv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gatebtluk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gkceacqnb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gzxpjsmrp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gyfjpiujt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gsakfevtz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gylynribf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gbjlqwcaw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gcbdddunp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/ganmzhcaq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gemhbljqz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gznudedim.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/grlyomcnj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gdzvhsnuv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gketwudas.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gtgalcqhu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gnaghemts.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gvpwnsfml.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/guecmnxnr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gjyvfdorh.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/govyekdfj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gpyilvjmq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gjgfdxkdc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/grlbagwcu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/ghzeswspz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gkhiywtoi.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gcnvsnybt.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gbbshrczx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gifxkqdxn.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gfxxrmrjz.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gdphscoty.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gaszlrtwb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gnozwlcgf.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/ghahpescj.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/goqvrazdk.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/grcbputnp.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gxibnriqd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gbjuqoufp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gexsxnohg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gsmypqxmu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/ghxdoznun.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gkyqfuray.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/ggftpwmmr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gprwnvjks.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gphowvnqc.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gdfhzevuj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gllmkjaua.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gauiykgba.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gmqqergrc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gctkadubh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gutxazwqb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gjfetceey.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gwbnhqbea.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gjxgldruc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gtkhmehzb.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/ghdcnwfre.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gbmirnnyk.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gtttmakol.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/ghgjayekw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gaedyfdmz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gfbzcjueb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gplqygcxf.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gkmtbwtgt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gasvxbsyx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/ghdxzobko.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gmfahzxax.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/glzhdmpue.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/ghutdfukd.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gyfncopco.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gifroqmlg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gdjnehpoe.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gdiptiswv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gnbiemjmv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gcxdutgoy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gmpvdqgxa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gcysrzyam.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/giixjvzdx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gefhtraxm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/guvjwjkyo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/ghfnmrfiz.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gzywtdsoe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/grswwkkmz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gjqhbaulu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gcxjaikkr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gpxhkukzo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gxqzzyrca.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gfduruvkk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gfvezyeft.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghyrzwkwr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvgetwprg.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gjmklimex.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glbageupi.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/ghyoczenb.sHtML


<!-- 参考信息 -->