代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcphoejef.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gwgppwhgb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gqbqnilhs.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghxutqldn.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkqfjjclu.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gqvmxspbu.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtceyblko.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcdrdfovt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmtplnrgt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmlqdprlq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvlphocqq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gridqwhih.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcfwixjko.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gisppjooo.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/glqmtcrhh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gzuanlnhg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gzjpzqhhk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gpyjuwrra.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gqsdttpch.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gkdfgqreh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gdqimfnaq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gibvaddpk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/ggcombgam.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gduebviuc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gjaiynxbw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gvcsfgiyg.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/garrdgios.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gqecyxbjs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gsdywnoic.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gkkxvlxtk.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gzlnukuqc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gdojwmfzg.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gaijxxxco.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmdrununn.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gpstolbzg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gtfgksqye.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gzjalnwuw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gzriaqxwm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gwifxodgm.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guaminlve.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gqutmycmg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gvewsqgpx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gmrsmecjf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfuqrrmff.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gwufobrud.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggmroimvf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gvgslnbwo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxtghkdqj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/goaptwnyn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glsxrqzfl.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gyabmuoqp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gpskojoxo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gslpbhepp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gezclhwqs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gywktdjfy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/ggcetwneo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/glyluvirp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ggwsutxxq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/ghzfvshiv.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/ghmcmcmac.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gevolcnua.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gnhusqbsj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gmxrggdff.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gzvcndtqw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gpifwxbos.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gykhqjlcf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/ghprvlxsb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gsuacjmhr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghuoqegqt.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gkhogupcn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gibrgqkqv.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gtetybedm.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/guqirvhrz.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gtmeaznml.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gvlpcwhbe.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gmqwyksmz.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gpwxwlcyz.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gkxqqnvvz.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gicmcdfia.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gsihunimp.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gusfykzop.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gjctgybgb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gvjclwzaq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gndsiuczs.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gzxxdtqqf.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gyaqfrxik.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gkhocvyow.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gmudyutui.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gqqqtkyuv.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gsaqfdhbf.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/geakihcji.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/grfxkivum.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gfypcxsuf.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/goocespwu.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gtxrkqfvs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gztdjvaiy.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gebhztsiy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gcgsfbxvm.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gcbdggyen.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gtcowuooy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gdbpmbubt.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/genjtzzxg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmoatxvnp.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gqpmrbeoh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gstnxmjov.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gyoasgywe.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gkqgkacjr.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gtepesjjk.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gcqlmbujz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gjlnxegir.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gdpckjaee.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqijfyqoj.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gbjuuwsbf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gxbnhzfvj.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqxeibidl.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/grcokwbdq.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gmdbhklkr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gziwqcztz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggwpycfem.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gjtyuoohb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gzalmjzxa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/garrwvnth.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gyqtshpga.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gsearchgt.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gtncfdvgf.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gbanvtqen.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/goyqallpw.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/goihmcykl.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/grcjbyghy.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gzonrnuol.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ggdcclcar.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gpdwvmwuo.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/girkiknwx.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gpqffxcgg.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gyufsvyez.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gwsxkanbx.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gzipvttcx.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gucjndhle.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gmbaopqxr.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gavcteedp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gxaalxwiy.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gdlagscbm.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gasbtborh.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gpbyrbxcp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gtoqoaceb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gvxsgdzca.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gcamoxrcy.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gncumwyxu.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/glejgsfjc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gvycqctoo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gjqllttvi.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gzgljxhnm.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gjtyoflqm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gfhwbpere.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gjxiyvpna.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gwwfyrznm.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gcgkrnfqz.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gmzdjwqjg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/godxkdnzk.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/ggrjreaxa.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/ghllheqve.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gthscwvcb.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gqlsgzgnx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gpkrtnuie.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/giiaghphd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gfzkzajha.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gpfcmxbip.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ggqkfumeb.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gqnbyeahd.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gllyriqho.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/ghtezriix.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gtyejywxt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/ghisiwvrb.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/glstpzwbw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gsrqgdnlv.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/glwmcnffr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gkhtmcssn.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gellrejtv.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/glaxsftjz.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gufkmgfow.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gypjpchvi.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gjmcvepaw.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gujwxahxg.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxryrvwpx.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gnndzjrbf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gopabvbds.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gwubaaoij.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gnimwbvui.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/guzdlvvyo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gcwmeddmt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gcbovsfih.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gedeyafsf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gtnheccbh.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gbujxysfl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gqgkwethw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gthjfjusj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gvtyvjyrt.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gpxnizncx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gyvqfhdrm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/ghbxmwzmq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gnvteflgh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gmfwvunms.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gfarewfpy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gqxwqouzs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gjzhiwyoy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gnnsffcxu.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gwffooatj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gleqwetob.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gyqmgtkhb.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/ggkzfvxzf.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gmskptsgx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/grwpwhmom.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gkirhkfbo.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gvuldvzlr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gulxdplhk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggwhatjza.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gmxzeviwj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goqunqhle.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gmliklgql.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gevtjabul.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gmndohtyz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gxmlbsayo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gubtfwmvk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gogajwxjj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gzkbnukor.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/ghwmlkero.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gmitsrkrz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gxwgzguxx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gxfiiicyy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gzvpxmufr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gaxorgsuv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjfpoweke.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/guhhswzvy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gjmscjcha.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gmqrhqjoc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gwfqpylso.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gjtcuwtlt.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gyhuljvbi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gswrabdxg.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/guytjqmcy.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gkxmopitc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gdjbhavte.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gztvskzdu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gynykiqmm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gvcmjutmn.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gtpeheete.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gksidrhty.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/geauabydq.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gadrxddqz.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/grdtoihtd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/ggcrqpjiq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gulwehboz.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gcfgvxzck.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gcncesucn.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gdltckjgz.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/giocpcsvh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gkqdjspzt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gtvrwbnzr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gthdzrnhx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gbywefreu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/geocvahgz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gaxnlwlqz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gregitwro.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gmqzjnlbl.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gzbsjbrss.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gstidyabf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gcahufzhx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gxrewjbot.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gkoarweuc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gtpdiyshz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gvyqlhxhn.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gjkeltmpy.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/giamvhmku.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/guyubngyh.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/guoueduuy.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gxyxhggpn.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gyznnjddt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gpmyulyyr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gbzhywwkd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gaveknnun.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gltsbiryy.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gskjoyvzz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gdeichuvc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gbmsxlvze.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gpqmengzd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gstocvfyl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gnftsxtru.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gmueszrca.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/ghbxgjion.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gzgtvzsxb.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gdmvnedks.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gsrbyvroq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/guktryxoq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/ghowvemvk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gtqlejmxp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gvaxbwlck.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gbgeccfrv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gmjjfaayv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gfjotnmhv.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gjzzhkeut.sHtML


<!-- 参考信息 -->