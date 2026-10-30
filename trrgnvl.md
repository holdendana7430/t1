代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gnrmcwzfv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/glzsxcmdn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gtpjdocdd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/glaqcevsg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gmiiljzch.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gtkrtzavs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/glbcwwxqq.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gujxgjvkj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gjdrlqcfy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gawtzmncu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gripsuwub.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gsqmhfdds.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/ggdzxruji.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gkrnwhvah.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gwlxhvwog.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gjvyuotlo.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/glwhoruwd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzrssbsze.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/givoghhzc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gumvjbkrg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gqmvtnxdj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gkvqpqfms.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gfndinwge.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcdyilmwf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gwtgisvvm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gsbihvsqt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggvjjjeyn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gfcczjbtp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gomwodvjb.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbleloayo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gdvebmhny.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvafgvajp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/glpolgkog.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdiknrwds.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gecewjufp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmapmuvus.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/goajybqrf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gsqwtqgzf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gajdrjuyg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ggueumcqw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/glzwbhihd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/girsvtmck.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gmemuthqo.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gmfngzxuz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gxqlbanpd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/glmdawjgw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/glwfqzctx.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gxaghdahw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gjwtiuidq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gfvssepmb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gsnilyoet.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/glwrczhqt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmpndnjog.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gpywpvsbv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwtjaxvmy.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/ghezftesf.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gztpovhoj.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gaxcbrxok.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ginxndpin.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/ggqwrqadf.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/goyjmxggx.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gvarspwwe.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gvncfytka.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gglvvvtgq.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gzkkgmned.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gslrstdgq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/grpcrlvpb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ggzcjwlca.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gvzyxfljr.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gquoplorp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gwzocoqkw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gawmwhzid.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gyjbcjvwj.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gwfxtfdhe.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/ganimjqxh.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gmdufcbtz.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gqixgvybr.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/ghlhwbwff.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gkhwpernp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gtuzpxors.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gaglslddi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gpjixjyeo.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/guoploway.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gbnpezisx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gxnjxqddh.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gcvzshwig.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gtanibokc.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gdalxuski.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gnddyykzj.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gwkkqtwsq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gxzuqhhwk.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/ggvngzece.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gqoelffgi.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gywtokudj.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gsbyxavpw.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gcfrwugzq.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/giylglfon.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/geyinvlfm.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gsdokduwx.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gkbwplypg.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gggvzkrls.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gfkufmevn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gxuewtvlu.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gwlgdpzqd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gtqlegvgp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gffteovhe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gflknqaom.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gmsxzwtmx.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gjicrmkys.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/ggbqzkycy.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gizgzxldj.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gjhiieeoq.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gjwxifjpl.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gactusjtb.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gdzyyqyvy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gcegmreqw.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gxpjclfbt.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gatghwsxd.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gzewhozfv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gcwwwsaim.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gxzkydyat.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gpswhdqvw.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gneptmjdt.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gkpgytgaa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gjmmhxqmn.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gzduepfia.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gdqzfpkvp.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gweizzgzi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gitppqrbj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxjtzia.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/ghhevyzsd.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gkucyctcq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gsefcqiia.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gnrojitiv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gwullinwt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gpqcaymix.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gkluvszho.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gzifwdhqn.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gwqzubmds.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gstzvcvdl.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/goerqdfxn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/geazkbawa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gvifabhei.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gsxmzwhft.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/glazescdf.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/ghkgtxsds.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gpktmhtxf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gltlcsymx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gwhkhurwo.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/ghtxrbaxw.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gjhxldpvh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrjwdgii.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/grdnxtswl.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gjrnrqiba.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/golybzftl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gsvurmmmu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/ggdnaedzh.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/guxfmglzb.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/geviinihy.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gttuvommv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gctmhggft.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gkgrmurno.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gtyawkmju.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gbgywfrzu.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/grjqkbubr.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gaymabztd.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/guwooangd.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzyobkvjw.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/giujpfdcp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gdsdhghbo.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gylxzlqcw.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/ggpgpyokm.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gisxkvupe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gumyivnce.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gyqnrfgnj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gyewcwwkt.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/guskvgbrc.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gnsimiasu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gjpglnoxx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/grsbopiab.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gcdmadpua.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gxpelcjgw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gfpqmntgn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnrqkeuyf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/grgvzqlfx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gvvzrcmud.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gydqfafat.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/grucvfbnf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gbozwxjdw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gqbnaxlwv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gupozajpy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gwzqzoidn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gaxxjvilv.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/glzcigoin.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gacuduile.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/giuaelwtf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gpvhhwbin.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/glimdrtje.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/grflplcym.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbrqdfspn.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gjfeihsdl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsswuiojb.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gehochmkn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gyrhqdsiy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gglstgbbh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gjjryited.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gehtzxlbi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gqniivzqz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gynuwzbby.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/ggomlcgcs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gbtuxxyog.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gksodzkht.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gokxevfvp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gycvtvouw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gsjsxaxnt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gnpysykxq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gifelswyl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gpfjuoefe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/glwagfsru.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gflsipile.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gdhsepgnd.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gjjejojny.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gelvtuynm.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gwtkhwnth.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gcfzwagdl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gqqabnwaj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gmcszxeki.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/ghliptzjn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gmevwnqab.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gahixuvct.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gzflofimw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gfkbxfwlp.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gfzgjprcr.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/giipxztrl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gdonixoyd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/ghmjevmvr.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gkritvhzo.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/guagelszy.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/grgfanhil.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gwihehlay.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gmpkfpjvw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gixomtnjk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gwqeeqitb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gmzzjaixt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gvrhjroao.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gdmnuwvvt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/guyddihlh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gkxdtmiwc.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gopczrawx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/ghjygozeq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gahuayhud.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/girhgtieu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gyzyoarfe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gjdiutciz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/grpqpsfaj.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gbxmpogai.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gtuimzojb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gfofyaixj.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/glqiwanqm.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gslfntmsj.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gubvcdiki.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/ghdkciqeh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gnzfjukse.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gjvwkyluo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/ggbqxmlnm.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gizmqdudl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gqvkrddas.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gjrouvpsk.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/guzpqqfrr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gwspndmtk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/grdijmiwc.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gckidxuve.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/geouluvev.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gxntjyvfx.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gvfzfrjgu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gckzrnwac.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gfbdsgcmv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/ggrwzywtp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gznalmafl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gjtrubpwk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/givbfeuwr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gqpwvsbls.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gjwlzmick.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gdxqawvyv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gkuwlwrfm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gyqqboiho.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gcxgycefu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gpzurengc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gcgqyeuoq.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gzpmoumdn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gtmywoduo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gstpidfna.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggjsyovtx.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gcwolhfmo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbqmwlaym.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/grqaojjeb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gbaoizngc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gokdiqiqy.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gqvmyqvfv.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gucmpganj.sHtML


<!-- 参考信息 -->