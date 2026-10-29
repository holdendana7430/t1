代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/grxwgqzxv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/guxwunpam.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gthazvjon.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmcxhdusf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goejcgjae.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gbwjhvucr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gmqbfpbuw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfkjnrgdk.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcnftigif.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gvicoyton.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfykywjbe.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyxgrfiyo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gceexftrg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giknfsmie.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gghqbgilf.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvfyixsuq.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gexauwuiy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjgrtvwkd.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gqetnaogg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gnnpvdhyq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gvhqqryne.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gifyvcgeu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gcuxyvjav.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvnsfgmfi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gqincgmrm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gyxorvvfs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gedzunrrb.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gizmuhowt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/goprjaixv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gyoeuzzzu.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gzdrxoqmn.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/giqfyvjbp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gjjclekks.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gnynylyml.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/glttdiebm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gddlqjamr.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gvdosiefv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbrwcrbvb.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmvlwzrss.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gziodwxmb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gizesppha.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/grillohxb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gtvmhwkls.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjqtlunon.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gekrqtych.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gwuourlpe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpgpxoetl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gtynheyyj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gofgakhwk.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gqbdpqhxw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/ghlwzszvn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtodohzrf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcrislfmt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gytwlhrqt.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/ghcbdpxtr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/govlmqakh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gafcuuifx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqofndjbi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gicuulibr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gkfgqbubw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gpyjeyeoz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggcvoouam.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gjzvqwboq.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gucubufvq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gospbmqiw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/ghfoqdldt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gpqkfljlr.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gkvsgssei.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gejamkwsx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gawaaggfy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gjsyapdtq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gebqsbzaj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbrwnuzde.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/goujiulkh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbljslxuf.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gaicpjmkv.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gggtyugrg.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/goeuccecv.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqotrrlud.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/garjzqqye.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gyvawucyj.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gpvzmyjts.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gyxjqczlq.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gobokwpot.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gxplnkunj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/goctllqgs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gjftuakzr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gxzoksucf.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gsvucgcnt.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gyqiowwgp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gtufisnxg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gqllcxzyj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gtbvtqawy.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gakoxywql.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gqbanlswk.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gimjcxwba.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gsurouelj.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gjlpvmjhk.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/glaonwdnh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gbplczaho.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/grtbuzjmh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gbsiziirz.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gusmnbvkj.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gkceprzui.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/glvronwpv.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gvfeewclr.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gdkqriuci.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gaqcajalh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/ghtmmbonq.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gpvoszbkv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gilefmiux.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gmicgvwgv.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gifbvndjv.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwlahdxhz.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/ghwjjpiss.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gnqhqnxll.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gunymigtf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gwnnrwuvl.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnbecmbfy.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/giypfdoiu.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/grffkgvzp.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gbghemenb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gwfxeuuol.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/grjlewhkj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gjtjjksxn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gftptpioy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gykazouhl.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gukcapuun.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gfgmqlusi.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gwzqiwwsl.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gltmrdrrq.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gjkanmitv.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gdovkozcw.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gtseebunm.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gzejpifma.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gjdumsiia.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gsblxknqr.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gesqsteld.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gjivokehy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gzqnogpvk.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gomckhyks.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gzxhxdcxk.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gfhsubgwk.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gbuxfcbqq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gzsrgimwv.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gissoditw.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gpnkgyiil.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gckfhagsm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gmgqydunb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gkllmesux.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/goormtcwt.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gellbsjww.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gqqvxdvpw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gqkhdsnvs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gabttnovy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gdmyutuoy.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gxakwjmtb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gagzdwdyz.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gqebgumbd.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gkispbnvd.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/glvqmvrpt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gutehncfp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gvxdcblvo.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gwgyiaajf.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gdlhgpbtk.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gwpktfnrf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gcihbnvcj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/glbaxjsbb.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gdqzzdozc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gyrlxazox.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/grxeavjpb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gpbronmwm.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gwikhsehw.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gqghzsayp.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gabdvtwzc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gohubpeps.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gofkbauae.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gcsggncnh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gxwgurbre.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gmrkjbjdd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ggfcqgeoo.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbsowyrfu.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gmuunayfl.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gukubpzgj.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gsxrtnrkj.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gweobdwur.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gjckudhwn.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ghxtpojyl.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gozmghize.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gnoezqwem.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gggyjqscg.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gzvciyfrg.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gyavbqgud.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gcbiscftq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/guuswshhi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/geukyneuh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gpcjmikva.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gfqnmhddb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gncspapos.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/ggmjyqjzf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gdizdkmqc.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/geubhntjn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/ggriiqwrw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gqeabljxk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gekpnntbx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/grziyupsv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/ghqdenlin.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gzeyldmmf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gzzadzbtc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gzptssatz.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gtlyojqxg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gdcaijtfn.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gnazyeqih.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gncudbypp.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gcuxmusku.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gkccbmdyn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gxovqlvsu.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gvbrmqyvl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/goegcamsf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gahdkoknw.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gbkcswsej.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/govvyftov.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gcrxnsabn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/guxnorgtu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gewwosgzk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gnverzcpu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gjzgstdjz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gkhksazux.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gycwznnhe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gxxhrurtj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gdibbchkq.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gageebdqy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gssuecdrm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gnvtztgsn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gfxktgthk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gvhufyjye.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gcbreqfrp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gtvybwuvu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gxrmxblxm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gnoqyksbi.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gdugfmnlh.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/ghoyjgwtl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/giwuobywu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gvychyaqo.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gyviflhkj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gnmjknetu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gryoofyxz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/ggfbfolur.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gdqyiuhte.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gjtkdqrnr.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gzauskimx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gqpeuumtl.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/ggzqhiqjm.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gsmewovub.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gqvnahkdi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gnhoclmxo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gqodgxsch.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gnxqflxti.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gyjtugrzd.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gnczridic.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gqviiwdxf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/grcbcvwbd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gxpcstfaf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gqphazhwn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gtyjddhic.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gstzpgijq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gitcsnxcv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gqxzljpcl.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gvwgkeeha.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gsfuucwmw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gymrxktvl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gpjakxcty.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/guucjczap.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gnvgpkefd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gikvokpjy.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/grarozidn.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/glusilkft.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gfhzamdjx.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/glljkrxlm.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gslsripaq.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/glvvvykhk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gnmlicmgd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/goupselrx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gafhhdhpq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gjtahnrvw.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gzgtbwcqe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gczsmrtzj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/gbtmuekon.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gniqcylen.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/ghjcbakbg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gorrtuhfk.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gavohqeem.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gowmerlgy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gojsrvdqe.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/ghdkikeiw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gcexagcnc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/grxndthyc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gajbmnauh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gmqwzaure.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gengrddqk.sHtML


<!-- 参考信息 -->