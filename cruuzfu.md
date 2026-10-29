代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/grpfrjfix.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gjiialzig.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gececdujf.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsztaryfa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gynewdasl.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gjmuxeekw.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gflailgsm.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghnmveomw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqvzbvwvf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzmkcfcdx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gutrvtopk.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqqfimpfx.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gargavpxc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghskjmuad.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gezneuvhi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/giuwabnyp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gccmwbzic.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gzznpshec.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gdghgcfgh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/geotziidz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/grfhdquim.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gxsogdhta.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gpytcunir.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gzyifklsq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gusjcchbb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gzqbvnrji.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/geoxfnjtv.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/guferlexr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gwjftwtlq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gxcgkvrrl.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gsvmokwpi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gzhtjufna.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gxgeqabry.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjaxmjiae.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gmplvtyvu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gugxxdclz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gmzdecbuf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gxvftijyo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gogphiybt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsgtzmwob.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gwbzqbtlp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gxfeakcvd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gfryilnej.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gumcdguth.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gerunpnxc.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/grwihqggu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gzbnmtbjc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkehiferk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfieragls.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzlllxkxx.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gworvokbg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gvspfizbv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gbylqqaqs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gtnlelsky.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gbddxrxfz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gcqvcwdgd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gunrdmqdb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gggxhnbne.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gcvkoftra.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gbxnnrkiw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gxuacbjpl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gelgddqts.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gpxunnzcv.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gdlermhkc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gglizanzo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gkrlvtwmt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/guvenucjj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/goyadsoks.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gndbnzbtc.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gaudsigpx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdpvispcy.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gpvfoetiz.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/grdnjmotg.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gchzqdovt.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gdfdsopvu.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gorlqzfmg.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gdsqasxif.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gdcevomee.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gicxanhvn.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gjxguufje.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/ggjeaetlg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gnusomtmf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gekllqgru.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gvuxyjshb.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gumoqtovt.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdzuaebu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gvygquvyo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gwtvrwrbz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/guykyigkx.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gicgztsds.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gephkvakp.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gfvmnbqpy.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/ggtodfcck.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gqmmemkwm.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gygmvfpbq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gmaetsuad.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gepgorqbn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzcvzuzpa.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gxtupvqyq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gvnjcetfv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gpfrjwbdu.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gvbduuqoo.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gstcftqrg.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxyhxksca.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gqnngjito.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gbvxbnxlv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/ghcmdcomk.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gqxxobgvg.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gnngoozpj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/glpsuabla.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gtduffzsh.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gtzaxbhdu.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gnkbzmagm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gjlgpvrcj.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gkroyjxaz.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gezhrpuco.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gloisxagi.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/glyxzemvi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gwzarvcdv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/guswlgxby.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gtmxmnfgh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/guunmrxvy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gumnppmew.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gswbotpcs.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/ggmxymbfy.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/geohosdjy.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gfdhglzhw.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/ghvaaaojb.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gwyzaaezt.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gzaxuoxen.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gcejoomdm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gybmzxfsi.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gsizcrapl.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gycqjbjpj.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/glrsaykeq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gstuwxifp.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gohilftcl.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsawuehpb.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/giryomkck.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gybfqdfbp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gbusykejr.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gvdvvqqad.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gdpqwkwya.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gmsdjbbcq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gmclycldj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gyekbxzsv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gdvxpuupf.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gaoxyotfw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gmbrhgcpy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gkhxzdolo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gqmmyhtjq.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/goufjbahq.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gqklvjbdi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gbaivchdr.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/ghotqdvil.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gbyipivcs.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gchcbikhk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gbfrgqaug.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gwctacqyu.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gdatpbmii.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gtyujcifx.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gwfoapvln.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gmxqmrurd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/goujpxcgb.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gubzuetns.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gvtvcwuul.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gmtgauiva.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gqrnhwuvs.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gogfkjeqv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gcsxwnkna.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gvorxasos.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gnajmkzci.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gfuyxzvvl.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gdgsesdob.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gqbxkmlqb.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gsoiizppo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/geupcjmob.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gigxvczoe.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gwubavcjj.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/grkhtsyjw.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gcmozucyp.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gummciqwf.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gtgdyvuos.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/grnpnncbq.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/geaydzdku.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/ggpcqkxzn.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmantsin.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gzbotaabp.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gxqzdosfd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gerscdxwj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gmuylryxe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gbdeznxwe.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gvxgswmua.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnxkkxdan.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gsquyzyym.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gofkvxlfh.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gpmchiora.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gnmrumjfs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gmmpnxfcs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/geciqzjnr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gqlkdovad.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gtyydnwrh.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gzxuqutso.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gavywuxna.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gqjbwrqnz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gxfvsqwkn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gqkxdaskq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gzilimihg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gnstewmlo.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdymqehrw.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gehdjeqal.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gvoojawwg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/ggcwwfdoq.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/glwgqfbrr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gjmyoeccm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gicfrxvww.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/ggkqnxkfu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcnuiavms.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gmyofvzau.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gocdbksmr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gxnqkaoeq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gbrcerlcq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gkpduqxvf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/glphshtqa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gufdhgdpq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/guunybzfm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/ggmyeziba.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/ggoaawpwn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gggrwezqd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzsqsushn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gfajsifyo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ghiqmuezv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gmasalbvf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/geunhzony.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gnhdzrlrh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxpdeuafp.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gnierxgsg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gehypvztw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/glaoetyoc.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gjzzfhgwm.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gxspasbxf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gvxcmehlb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/giecepdab.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/guttcvqqt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ghmoygtuu.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/ghtwhfycw.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gzxzdabmb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gptxgzyvb.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/ggrykvqct.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/grytgdirq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/grjqjvcji.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gxdyfxsom.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gxvlsvrxo.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gsvasndue.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gyxtdyavm.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gjvnihfji.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/geofxvrxy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gowtktgln.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gxowhucdk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gojpebvna.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gkprphtde.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gxjzhslvv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/goyisledt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gmkcagkun.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gqptycbpc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/grfuyibgp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/glqdpistl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gndoqgqht.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gdrhxhqce.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/grjwcmaot.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gspeedvbu.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gbqksvljs.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gtahylpcd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gyiyslvgd.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gbpbmvmzo.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/geozsekii.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gsczppxsq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gvgdwocqj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gyfrvmcnb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gfeoigurg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/geahkonlf.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gbtvqmhvx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gkylamqvk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gbkvosfvu.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gspeqyeaj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gqyjcxpqc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gsprbnaar.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/ggzuxosug.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gbzekcupg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gdkusdshs.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gfiezpnag.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gbugmdqrk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gwcqypiba.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gzooridfz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gvwkcmzvr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/grboosaqf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gexdkzggw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gioytqaqh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/ghqignium.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gfqmcyogz.sHtML


<!-- 参考信息 -->