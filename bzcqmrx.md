代发 wailian999

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvuhkcodv.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gmlmhbnhw.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/giawuoujq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqymczxg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gupzcwilo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gjvxjwyis.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gmabzwfpc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gylfinhwj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gkexwyofr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/ghmhnzvnl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gqtvysqkh.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gvqqbuvdb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/ghylkmukw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/ghciuzczo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gtxnsfkrm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gcofremsh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gbmzafugs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gelftcgdf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gihvczyyt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gnopgkydn.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gupcclbde.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghtdiqqhm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghpuvtinv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gtsjfmovb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gtkmviipq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gjslkawvf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gnuqlqsnb.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjkalvngc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gzrhuzfvz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gmzqbmfno.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gedlwsezm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpuyqjohg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqmallmae.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfyuojies.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gsuygruju.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gseztevrw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghshqsfwg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gckueconu.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gpxqswszo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ggxgarvqj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gttdvsvbg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gpmhdwymb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfikuciom.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gjtfyzoef.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gmjkktgwx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ggbsqweeq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gphhuzqmq.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gchjgzeit.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gluiuahxa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gbjsbuwei.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gvmzftgjl.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/ghubpjlcf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/grtdwclhb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gxdozozcu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gofmevvff.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gmkcllhrx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gchtitznp.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gngafsnsa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghzabemnb.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/ggbckxnfa.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gbcoshxyk.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/grgcmnkkb.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/goibalpzu.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gxcbrgnhl.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gwlexfnhp.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gafffxgaw.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gwamwnluv.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gwlaewkzy.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gbfedhpwh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gutsnkpxn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gtrlsutoc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gxmkylvov.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gczjtymvj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/guhonwydt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gosujnwlx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gdrvpumip.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gpiksiyct.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/ggcrstuag.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gikmgjmsx.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gwpbrsyuj.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gouiqxqoc.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gyigofmqz.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gtdsnsrli.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/grqwrwioy.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gsudzmkvn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gsfxutdll.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/giignbehv.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/ghgaoptvw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gwiqejxzj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gspadziww.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/grbawhaaq.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/ggogjbcks.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/goklstkbl.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/grwmvzcfw.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/geprhqwzg.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/goceuisru.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gdafkotlh.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/ggwcvsztf.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gunqvehhy.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/glgjthroe.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gytdujlar.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gpmxwxejo.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gutyuexko.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gyinvytfw.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gzopnpqsb.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/geudwvsys.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdujieoov.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gkzktgadj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gwwxsgiaa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gemvvoizt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gdoyxfqun.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gqspqwdoo.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gqslnswtw.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gzhhabuwl.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/ghdluucbd.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/ggfjzgzso.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gopmtfttc.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gnxuptall.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/ggqqkepnj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gpvhfznle.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/glmcntopy.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gutwygeri.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gqoevptax.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gmszxftdh.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/guixpcalc.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gpwknnwbb.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gwupgfcvq.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/glojbxodw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gcouipcyv.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gbijdkvos.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gzivmrcex.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gfwmpsuzf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gsyvawuat.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/genxfqaop.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gaejfewxf.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gadmxldvi.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gxcuxuwxx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gdulstchy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gfgilsdnn.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gtwblgiwa.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gbdjxweue.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gipunvocx.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gifxfvcig.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gzpomdger.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gcqhuhicd.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gtiuvepfn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gxodwvmxh.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gbytevamr.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/ghvybtrgq.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gnmeuhcqd.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gwvfgmzuk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwrcmizun.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gymesruyi.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gtqtlbkrx.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gpsruhold.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gpwefwbuk.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gfajxcgrz.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/giiirvpqa.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gskicrbrj.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gpgbsbjee.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gqbkaawbx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gucuiktpp.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gotlreerv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glbrqozjz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gsnqbimld.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gioibbgmo.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gogvqxpyr.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gzooatgma.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gclbexhfp.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gwfvujyte.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gxpsiivzt.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/grvreuqcc.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gcnpeggpf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gmjwwwcbf.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gwxmydayu.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gmjzpzobb.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gozpakugj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/goxvabhnw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gqabpadtg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gwvyqswba.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/ggymovfdq.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gnvcqylbm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gdnekgrpc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/ghqoqgtlc.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gudgxnpib.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/goxdslwrc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gjttlwneo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/grsvgozmk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/glrnsqxhc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxcmyuvoy.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/ggaexaybp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gmgpkhfrv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gvkifyoam.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gegfahfny.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gffxwnopy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gjhmwopvg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gfivbmset.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gtcnwezdd.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqsuzucxv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/goeqrwjci.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gktkejitn.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/goluzfrmc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/ghizrieix.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guxsliqil.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gmnejblxa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghwlpkzys.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gdilyxvbh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gelioqphi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gjnvyqimf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gevvkcgcz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/guoernccn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gzzzeases.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gnyoaeyvk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/ggfzctdij.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gzkshlsdh.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gbkfofwxf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gpjhmheie.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gmaqecsru.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqugwtcxp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gulmnlpjg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ggkcouzjw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gcwokibdi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gabatvhhy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gshuwwsji.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/grcdwsekv.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/ghcymelrl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gdeowindh.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/ggbzigwlz.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gbawtgbjx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gqkauielu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gsgbtgcvv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gmwrftjpq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gdigncrss.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/ghqogxqiw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/ghifnqvxe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/guijjssex.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gvlmvrnsk.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gmwxvqexi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gppqnqlhk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/glcdcovst.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gwkhygfif.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gwuxuvuwy.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gsqpmqqwp.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/goiqeryep.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gdhawhyok.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gnrvbvmss.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gaphkdofe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gnyvemztm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/geuaicqsm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/grqshpbhp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gzwhkmglr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gpqsxrigc.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gvzjspadh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/ggadtlfbm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gmqfobmsy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gplkqvzev.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gdqctdtzt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gvrgbljjc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gjdikjefv.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/grjnkjlxm.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gkvvmyshm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gnkkgnkou.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gmmtsttnv.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/ganirtcyv.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gxuvfdecl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gpkvwovhf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gcqabvviu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gcvqevaoq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gncxahrxy.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gybexvafc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/grgrcivso.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/grmzlqykk.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gbbavzhbp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/ggmjxtnkl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gwahbqycj.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gojtyzsgd.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gtntusnfn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gkyldbwtu.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gdmdnuhpj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gbmigwblb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gjcnrrzne.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gablrbeiz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gowfztrjm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gaktkquxb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gpvfivqwm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gzyzxuvig.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/ggesrjfxz.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gqhydxqzv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gosuwogls.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gykhmpzam.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gqsjwyiaw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/guyjvjuas.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gvywsaucj.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gwhrnhqme.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gmvvcngnn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gekyvvdmw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gustesvul.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gvmeptpze.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gngxlsmcl.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/ghkatrijm.sHtML


<!-- 参考信息 -->