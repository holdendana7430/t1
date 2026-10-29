代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gycedvdxx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/grjdthyzi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gijyqkela.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gjkzvrmqm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/groyspmqo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gkuuvdlkm.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/goscjcjnh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdgzpeyyr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbgxpnook.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gvklswkjm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gwdsqseig.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdtdkjvae.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcxjdmixn.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gcbohfnmd.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvcbvjtqe.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gyhjoripd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfpjhlech.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/goaknxtnm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gwvbtnmyc.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwmxxflum.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghqciyyva.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcdashftj.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gmnhhasmg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gvlfmgprx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gzocdxqxc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gxvwgpgdo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gjfkhityv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gegttnbfs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/ghpxgrjlg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/grgkswvce.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gyvpcdewh.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gigtopvds.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gjkqoqzka.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/ggvwlrsrr.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gdqmoplqp.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gdhuhoyag.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gzbauvqeh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gnapzabyl.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gwbcsmjjl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gshfdznhc.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gpsiymmkl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guthzqvoi.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/guhjhbcnd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gyynmkbrq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gphtohcnl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ghmarjkac.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gdcsuutuw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guwncyqti.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gbyqcdmli.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/govprimlt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjghsgknn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/glpzrpesu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdvdfxgua.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyqfqsfbh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/ghossnkkn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfpwxpswv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjyieyhfe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyfzkvuub.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gegngrkgz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ghhvkpcts.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/godkedebv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ghqhbcfqi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gagzpeorj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/ggpdjizba.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gdmknmmor.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbdurfqno.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/ghacpsmul.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gnkvyxtoe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/ggpcbswyq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/ghrrwetzb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gkghryxud.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gbsdouvkf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gjkexdjwp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gsepzzpmz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gpelifgfs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gpnlfhfcm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gygfkabid.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gmdpyeikg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjgvtpovi.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gwbrcqucl.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/glrlabpxe.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gdnsyyvdv.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gcbwzhiot.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gysvgshdw.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/ggduxcjzj.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gxbhifadi.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gppcykxwo.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gmtrtcsml.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gbtovpbch.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/giacjsqyw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggzelgauj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gzocwhkkk.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gdwwkilmz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gxiwskvkw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gubhncbpj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gtzjfmahb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/glcifmttg.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gnkbkzxlp.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/guomevfsy.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgjwonb.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gvlmvuxrb.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gskipuwhg.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gkrwonirr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/grujommeu.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gusxeyhhh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gefcurlhz.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gowxyyhhj.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gtxkduouh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gfamntfxu.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gvvpegxoy.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/getlanrnw.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gltgvirgd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gcmsgsaox.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gpaseewvb.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gjjqydvfg.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gzyseyjmo.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gwcohdmuo.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gklspsdtx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/grrxwzeey.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gyusrzhfg.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gtudboxvp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gzckwjfzk.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gjmyzyigp.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gytkxngly.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gxxnlhtsh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gtaeaakbd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gppyjjify.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gmuyzgwaz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gvtmiisqe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gdqdpinte.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gjobklqkl.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gyzsycthm.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/ghzjfdale.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/godsgkcje.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gbqvdjhxp.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gqgljejjj.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gxdvbxrij.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gdosdsiuu.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxnyzjbsn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gmqvrmytw.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/ggwftcszy.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/ghezrfeva.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gnfbmmjut.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gbasbhjlt.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gwvjwajkg.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gitgtjijj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gnjoypttx.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gonyfqlut.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/grcdgitng.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/ghfvxuepc.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gvprpwuvh.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gyntdhezp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gtsqbyute.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/givwsixku.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/grjofkepu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/giaeuhicz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/ggrdqitlt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/ggyoupzuh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gfbxzrwxq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjtfrlglp.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/glpzzfleq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/ghjwdfjch.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gnxuecayj.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gxcwggtch.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gbditllqn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gnqtlgfqy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gvcqmqxnu.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gijhnuxjp.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/ggfcpxzyn.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gxhwdwjbx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gbfttxnfd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gengggcpk.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/guhqazpms.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/ggweijfbs.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gkhwbpdca.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/giwnmmqtd.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/glgorouek.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gqbzlakzx.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/giedninwr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gzfcxvapg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gerkrjksg.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gnxllyxxu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggunakjsl.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gbmgejkfu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gmkbihsrp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/glovabhcg.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gxxtuwpvg.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/ghdnvlifn.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gzgnfcegc.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ganogemze.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gkvwbkhmq.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gisvxmann.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gserzvjzx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gbllpddjw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gnfvlirfh.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gxklkmena.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gotqmlzgb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gluhicrsk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gcadvpzyo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gqpeugutk.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gvjpdcxxp.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/guynaywbo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gpppljscu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gvsyvwcuo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gquagrnzw.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gyxwfjqyh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gkjvtmxsh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gwfydgheq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gzgodwidj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gzxudzjko.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gkzqjwfve.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/glypmdovv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gixnhlrkw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gvqzwpghs.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gyrczqbwt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/goqmizxrd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/ghzkxexqt.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gykccdmzw.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/ghbakfayp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/goizssmkr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gyhnvqufg.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gpymrrlyn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gqkonolbv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmcuhagia.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/grhxxdjax.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grgkdoezi.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/ggvjzhooa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gnxwvdbez.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gmvwinygu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gbzkffbue.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gwfgjrqzz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gqklcfwqu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gxdwbqjjh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gxsijodly.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gpjxpybpi.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gxzzxivtl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gzkigsefb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gqotogchs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gohsfyimd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmjqggjhk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gprvyncva.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gagdimtno.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gyqiiwnuz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gjkimaeqv.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gxgxrnsjo.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gdozwhohe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gkbzjrrrq.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gwgnnepwn.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/glewynubi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gwfnlxevp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/glkswpquh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gumdpmkvh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gbtgylljj.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gajaiaykd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gfgehmxbx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/grfotqavv.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gggykeppd.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/giwkbpvfn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/ghkfvbwqv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gqlptmupp.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gbfiuruwx.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gjzxpfuxa.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gajwwftlm.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/grgbhmded.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gvsscphin.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gowpfjtmy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/ghoubnusx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gwgdehxsf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gpsizsnft.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gioakyysm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/genoxvecy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/ggjttmmsp.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gdygbrsix.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gaplnsnga.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gpzjvsqvh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gysbrdqtp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gukzvdjdy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gcknyqtsl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gxykbpbnf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gesnyldzi.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/getvtmbql.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gwymcjkkd.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gvtixcqqa.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gdtoiejcu.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gkrbiwjvr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gwfhrmnkq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/grmovafjr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gtbhuzvua.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gbqfiyoxy.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/giidxokqq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/ghufhqmnp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gaqbwekoy.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gtsfzzahu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gfqglaijj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/guiaqxaxn.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gewnfwkbu.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gtpsvojee.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gjogtnuae.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gxpyvxknk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gccjvqjpe.sHtML


<!-- 参考信息 -->