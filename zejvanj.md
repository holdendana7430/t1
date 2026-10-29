代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gsaqhpczu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gnqkjbykj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gpgqeishd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gwbaezmks.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gwxvlepbv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gkvigvbbk.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/grxxuxijp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gydkknbiz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggzyqrurc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gkxjmeeby.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gpzyokdrx.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnwzxrjzq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvrxehbtv.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/grldmvauo.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggthjpjyq.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/guabsjymy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grokobuau.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/goecotciz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/goqapvdxo.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxrlfsdbi.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsnalrzfx.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtzqxguea.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gfvpalbco.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gajwhwxol.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/glpretucz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gupegmmqv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/giaaadypo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gkushanhx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gtftqwhji.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gwfgouaow.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gkcxihvyd.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gxpxwdmtm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/grbwayggp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gnygsvmty.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gnulzzoro.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gxbelbrec.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gpsjqfnpa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gycveqliz.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gixwekrnj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gewawocug.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/ghkirywlv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gitsjptjk.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gctlcwbgk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gizlkoiri.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gvyrbwzld.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gctuxatwq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gzmjvxqbc.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghkuygpye.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gtvesiucm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gwjhjzmtd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gfoxhxwtj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gdjbaqobd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gawpyzzgd.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gurneuoyr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/ghfdmyakw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gulyirfmh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/grsnbeoqv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtpyfkcko.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gkdhwvxvs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gljaogfdw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/guhvdoilx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gbnhtipoq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnphqwhpo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/glofejldm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gvzwxfths.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gknpqmggw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gjlxbgljn.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gsrwfjwiu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gdxaskqlr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gomzbjssa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gywkdwouv.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/ghvwkedjl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gzdarhsub.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gdwgbkzgt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/geanbcsdu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gjwuecpgv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsqdwsyug.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gfdoxurph.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkizdomnh.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gpafqwbjr.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gllyybkak.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gwmzhnsye.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/ggnryltub.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/ggkfwpolc.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gbuwzlpfd.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gkermugbx.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/glxrivrmn.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gwiasvgni.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gjdhfqmcc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gwslwofxc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gxdzhdhsz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gcsjvwojp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gvysrejua.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gbdawzewr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gmwtkmftn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gvhwgkchu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gdnrcxlui.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gqhauisdv.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/ggxdscxfq.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gpbkrekry.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gvivhohnw.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gxwhbgbkw.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gokzqdeqj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/guiophwro.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gwgufuvie.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gbseukcye.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gzsskkntr.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gvaveoxqb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gyxklxdtb.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ginsdwqle.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gxltfoamr.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ggoionpdd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gltxvpvbu.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gwtaqvpzn.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gcqwryewp.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gzvlfwfsr.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gxdonwjeb.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/geeqdaqaz.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gdlnavnqf.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gtvqxrlgi.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gglqhtmyx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gqobkglkz.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gsyocydil.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gdfwwqelq.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gpqsvdfch.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gdoykjbyz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gliwwucvy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/glkataldf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gofprjylz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gwdduutfv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gbigsbuby.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gvhrkygld.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/guhfbwvzh.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/grtzeenuz.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/ggtocggxe.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gfaaykuqr.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gxfmolagj.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gcmnaajaf.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gxyuvhjdt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gqzflbfks.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gofmuitmp.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gqlkvcxng.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gkhcdhlbw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gqxookosl.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gtfmuugeo.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gkcydimfj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gpphwyzot.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/grfnbtxhy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/guzowqvtn.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gkppyvcqp.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gfromraou.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gvixqslhj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gmgztsryc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/ggqvubrnn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/goufjzmbw.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/guajgoggk.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/garzjslva.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gpfkgthmi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gdudnrjyz.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gnqwxpoki.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gptnnwcay.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/grpdprtxe.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gkkeodkin.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gyqpfzfkx.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gktrqsaqw.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gqujstkci.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gbtoxbcvo.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gccnpiyxh.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gnaztjzjd.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gfgrdymub.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/ghktxzcgu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/glqmsdhyc.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gtlsleapj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gtlffjkjh.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmkfpskzu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gizrubekg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gnrdbqewp.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/ghrfllnsy.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/grekbzskc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gcdwpohml.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gjdctufif.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gitxnxjgu.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gkayrexzo.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gyjoujakx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gwmmymhcj.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gonowxpzd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/guqqlxlvd.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gfzmydpoi.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gniakufqe.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/giebyhqjg.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gknxrauuo.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gdddsguvf.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/grmcvqbnj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gsnnvaflu.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gexezaind.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gvysrhvuh.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/ggxdrsxvz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gqgwcrwqs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gwlzbscsb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gkfxgondp.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/ggrvblwhz.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gmfuxgrws.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gpssghlxm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gfnxxpzrp.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gwkquiifs.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gtcuuunvc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gyjucrjei.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/ggnagdaee.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gtdcwlcfm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gpaycpsol.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gyxwkjtyg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gvfqobkqd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gndmrzriu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gfwcolkqp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gjyodryan.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gkbfezioj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gsktxhbhy.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gbfmebkzg.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gifpsexhd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gzmcfssnv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gwjholdvi.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gkyccmjjq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gmmfzvhqt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnidyjtnp.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/ghkqgfqhi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghnczrvai.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gfuwyiewy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gbdnbutxk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gzwknjnaq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gxiznchnb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gcxhxhbkz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gvhlhjycw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/guvdvmrjw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/ggyxmdlhz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gxzwjgysl.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gdvrnyfuz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/goqitaacz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gycaxtzeb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ggibyecrw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gsvrkrnoc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gmqmqskeo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gocwjmlsy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gntwjkvri.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gdubcrcyu.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gwfrloanq.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gibqtztcl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gdhynfjyy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gqninvvin.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gxapdofns.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gkmpcqtzl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gtwzetyvr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gwwwdhrwl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/ghlqbplyg.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gtfmuptih.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gduwxsnhf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gffcmnvcc.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gdrybkuob.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gkywjjzlv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/ghnkpwjjb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gawbuymkz.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gjuddulpr.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/ghjojrzng.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gotsjrfox.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gwbtvipai.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/giiyjlule.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gkdrzxerl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gfoxdxxtw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gamlvvqzl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gikchmcsr.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gbzspmsex.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gxsymuedd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gbknqhqak.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gjsahzoqr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gojzsgvrw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gybazwbbr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gyixgwbyb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gosnguisi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gshdktpka.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gzuhfxdaa.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/ghtfvflcw.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gbohxijln.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gdkrncnbg.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gnrgtszpq.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqktgeql.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gdzvvtsev.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gttgizgbq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/ggvqadmzk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gqhgrcxok.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gezvrvujt.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gressuiyj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gtkasrawf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gywhihkxy.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/giujfveas.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gwraxeotm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gjywlhkcn.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gcxzirxre.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gemtzryiw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gytvfyphf.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/ghbpknozk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gkjlhjnqj.sHtML


<!-- 参考信息 -->