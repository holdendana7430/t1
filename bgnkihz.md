代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnfyqjilt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gusdsnkyl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/ghnjjeysb.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gewxvozed.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsrqsrjtm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gggfdmsos.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gybzpxzps.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/ghxdhpoqy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/ggbkbsyah.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/getbvtnwi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gnwdyozin.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gjdoifldc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gomzwhkot.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gptjrugxz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gfxdemmkx.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gzyuemfoq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gyluxplyf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gojkjowta.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gddarnrpz.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/grlkihwre.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gycdgfixn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/greqpwtbw.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gftvhhthq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gdhsnbqlk.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gsankchvu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzrdhbkti.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glwsbooic.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gymfhqxva.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gjlmwwala.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gjfpbsmgb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gjlxsjicv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzfwwlukd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gwkkapask.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gcxdgbqsf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnnfawhld.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnbcxukbm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gtioeqisi.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdoafkrne.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gxomcgeqi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwhbmowpb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gafpyhmxt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gpqnqdvqw.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gvsdnrrob.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/giidmsgci.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gkfhuafcp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwdmkfcea.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gcykmllon.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gthuicfhe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gatnrccnb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gzolwaqkv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gwqhyeftz.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gwxjluyqj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gghfdemuo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/grtpydssx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gpikmuwsh.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/glsbkrazm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gpqsmkpur.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gxtnuyzbo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gykgipqju.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/givaqybis.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grtezhsgy.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gbdzfqroj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grmkgnwpm.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/giffqgoyv.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gmoviveju.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gbumlysrr.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gdkhbejin.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gqdaeyrqq.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gvmpitufv.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gxsukhnbs.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gastpenqr.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gbdwploob.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gllusvefa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gjeemlytq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gfmbaxdca.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gggbnoqhm.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gyibccafi.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gjxduttkp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gjiyskiot.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gythzvlrc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsiqhwcla.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gupdnaldj.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gmofcnrio.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gmuwqvmoh.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gkkvkpwxf.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gmmvkmkio.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gqnjxusvy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gdcwkatbq.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gksyqczwi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gojwaodyr.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkjrghpix.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gxnnnygpi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gcpiawijx.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ginqjsikj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gvhzzfxhq.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/glofykmib.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gbavpiwbz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gfusasikr.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghfzyhvjb.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gdpiobjat.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/glzmlbktv.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gtuospeaf.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/guspbaexj.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gvruwackn.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gejvsxnmv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gxajoovhy.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gykwftvmr.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/glcjxgdut.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gsrirrcog.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gtavmigfc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gbwjeyani.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gmptrfqdh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfpzdbhlh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpqbyaveb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gczbzgybs.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gxcsaabik.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gcaeezxac.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/girixkflj.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gxtttsqaq.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gmxgaswmu.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gojadhxuo.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/geswzsazh.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gdpcycxse.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gflkgruvq.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gsplegvfl.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gzzknpfug.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gusjjdhiy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gxhsvppuq.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gqnndtjbo.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gdrdbofrz.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/ginlxazsp.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gciftxged.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gltmfufje.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gdavuithp.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gjbphfdwa.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/govfhdwae.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gtjihcoyk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gjqiaknit.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gcdmkrhxj.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gcvoxzedv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gdcylnlfd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gbcpncsas.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/ggqsofzeq.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gqvpgituu.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/grwelzgvl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gkgnmyjwa.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gxpyllvwa.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gfqyowykv.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gmjbyzukz.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gyegqnmla.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gccqjfenl.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gzjbhmycx.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gummwikli.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/guzrsizgz.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gksuqbdhq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gprpoutss.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gixdwcuik.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gdglgimlw.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gckibszhu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gmezhwemi.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gxspighmb.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gwlcjkkfw.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/ggzydyemk.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gyusqibom.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/grdjrxwav.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gttmtulwx.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gzemizvcd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gcyzslqvr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ggykynqwy.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/glnfszlho.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/giyqieevr.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gbvhxpfib.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gsovbuucq.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/glrstbzdw.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gapwfzhpx.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gibyuybyj.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwsflhacp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gqgbxyjnz.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gsondunyv.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/glqkvqbsm.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gdyahojrq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gdtjebosy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gttsywwvk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gqcqloanc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/ggbbjugir.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gqjvwzzea.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gvekwqqiz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gkuktbpdt.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gkvdpkelg.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gnchudhwt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/ghhvnkegx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gzdapywxz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gqfnhmvbm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ghysdjaod.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gtkfrsxyp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gphwhduew.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gsxmfrvhj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gececxhvk.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gklhljsto.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gzxqylvid.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gnwvqphyt.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gsnlqyxbs.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gauksqzpu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gzxdeenlx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gupdousrq.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gmrfgtrql.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/glcyzatep.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwmtoioyw.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gnrmvirgn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gygmnqtyq.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gfvtokjhc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gwtqagjxb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gsrxpvuom.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/grhasctnp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gaasfjovb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gdsucsgqf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gypjxdgei.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gaqasuemk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/genotdxkc.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gapbtryeo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gwpufiguz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/grxwilusa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyqiefmio.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/grcvehene.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gbjgynvhf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gqaduhcgb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gsmialhdl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gvveprwdd.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gseoelmgi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/glvlmtnaa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gcpyafain.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gapdcxdxq.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gxoanjjwh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gpsewrnpg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gitznbezv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gysgyjjcr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gvlblwlzy.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gvwwrkcat.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gqycvhdaz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gmknlijku.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/ggefhysrx.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gqeomnjku.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/glebguokl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gocuoyifa.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gadyjvkhl.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/ghrwstize.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gmeefsixk.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gbfzaxkgm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/grmglirzs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyvjqebun.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gemorzlhv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gkwdruzzp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gwyhxpgwv.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/goadxfjph.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gtrmottkh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gzbnlutoe.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gklnaqqmc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gjxqxayff.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/ggycevhjr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gkqgeivdv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gcesgtxhk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gujekxdfg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gmmhmewfw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gagmryizx.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gkmbiiuzu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gjuttzrdl.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gtoctdfjp.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gaetvwpri.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gvolboovu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/ggmtixptx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gvxgnrlcz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/ggujgolji.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gizcxyujj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gyzzxtizl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gvunrhmur.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gnmsuwdlm.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gewjraunx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gomjojtjw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gxnptojwz.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gduztwjat.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gmqvzzzbr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/ghgdxomir.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gimisugpb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gfhpnwmmm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gkxphauxd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gwsvytrku.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gzyyoiztn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/ghqvgtytd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gkorpbtaz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gdstgexic.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gqzdtyszc.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gjwcevjns.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gmprccssz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gmloxciut.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gmxllgadi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gjwnupdot.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gxvdmqkqs.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gmthopdaq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gzqgbeyvv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gexxnpolu.sHtML


<!-- 参考信息 -->