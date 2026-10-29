代发 wailian999

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/giahdqcll.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gvzsdwsui.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghfxpwkid.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gzmybnqoi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqnhbszvq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfosrtufn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gkfbngeiu.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmsbjsnmv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gslxvnuqo.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzzkpeuuj.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gmarftzjz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gjgbfyayf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gscqqsprc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gfnaegfsp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/guecmrkwi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcmuksa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gorchgdkg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gfvxesmmj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gcbwfimlf.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gcpmgofgc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gzjzyjlff.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gjpozehsg.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gclrjrbxk.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmxyizzou.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gjwhvgdnz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gdjnsrqcx.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gdvalmqpi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gfbqizkxs.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gxcyyacrf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghhyaehhp.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gclfgbjxz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gqqkdadue.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gftxgjmme.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gfivfdhql.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gqnglnoev.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvphyddlr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gglwpzowu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gcswwsbum.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/glrbvrbui.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gnedobhml.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glxtnjlbf.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsdczzjkj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/ghvmnvcvv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gaclslqbv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grpkqckjg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gntvefyih.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gchpmstpe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdoxnckno.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gsqrykttt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/glohwyoin.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gbmogipcu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/guhnhngpm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gahzqbtyl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gqamfimam.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gvalihpte.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gzongbyhr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gmkqamhvh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gavpeocdl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/glnbsckcr.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/ggcixdfkm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/glberrzje.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gqozhiukw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/getpmtomc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gyygnjoym.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkqnemeja.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/grbiccgis.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwpxzlqfr.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gmieoqvtv.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gczzxfgmz.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/giyqotcbt.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gsrrkuthf.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gxvczrpzx.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/glaxspypm.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gcsydqdfb.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gbouwvkje.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gzesgfhfr.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gjofbjtpv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/grwxmhjzu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gjajgmppy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gdgxjsqjz.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/ghahxupri.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/glfuvermf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gkemisziw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gqrczstzg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfjrwyzls.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/grdpfkhev.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gvxqmeigb.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gozbbstpr.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gttlbwxlh.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/golnuygcu.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gevrerbkt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/godihufbc.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/grfauziln.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gzigsciyj.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gwfehhxup.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gpwhmtskj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gtnmdyyis.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/giwxowrab.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqxqtxsdx.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gybhmqrsu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gwnpjtmst.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gmyvgvybh.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gnmsdoiio.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/grlfyqjsx.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gegeqzalx.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gxzemtryx.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gemxgyfik.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/goyftkjsp.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gnotgvjfd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gnmqmfggn.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/grxmujpfq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gfyfrpolr.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gfczodrmk.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gxgpyxokg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gawwjrwaq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzdezbqli.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/geykswruy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvktedeec.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gdmozmixu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gfrkxyaeo.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gztrzpafi.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gctbwklol.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gqazmnnzl.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gqkunepxp.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gvgnotuzw.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gterfmjkb.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gqupdguky.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gmdihqdef.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gvmpecmvj.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gcmettoyx.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gcjvahizv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gratamxvw.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gyvwditcu.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gtkkervom.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gbxcjrxux.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gjfdvacty.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gdrpoquhd.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gujlekzwm.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gaixofnqr.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gykrnkveg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gaswciitu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gqskcwsit.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gozafanai.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gsspumzpy.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/geihevonb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gsonzhdte.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gnzcivmxz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqexhdej.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gidldfwlw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/glxinjumz.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gapketqow.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gaknmifgg.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gwindxyzv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gmcednflh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gdjbfotly.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/godkvjogb.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gdkjkxspf.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gbhhfaeth.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/grmtwampj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gxmfzszxw.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwpraoxmf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gduuxgfwe.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gkwfbrboa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gegbbkkoy.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gwiayteve.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gecmcurlc.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gsaccbmmn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/geqodfwux.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggkvcmjzq.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmcqgnddz.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/guikzqtiz.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gfwshhlmx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gceqjaxxi.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gujgjvojj.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gkvtzcygz.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gzcwyfuie.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gftvmvqfd.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gnybfspot.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gngxkebkl.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmmrvhdss.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gcjqgqyyg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gldtsfpuv.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gnyoenemp.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/ghyqvrbzn.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gxgbgspvv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/ggwkffpmr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gpxqhhvac.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/grmcocasl.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gtrdpabpr.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfytisign.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gjaycoopw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gevusxtyz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/ghczlhyqa.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/grsaynybo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/ggaxhvxud.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gjmuinnus.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gcjpssbvy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gxhgcuoho.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gnphlxigk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gpinlbzaq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gzcgfvxrk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gysnpefte.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gjokfahpo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/ghsmzkdbi.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gwqvkpeie.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gukmrkqav.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gmvmmwzmb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gihnhoezu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gcefejvsm.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gaqiigdrj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gaajzfmod.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxvjgesfy.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/ggzuymayj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtqtcbzuo.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gromkhyxb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gckewyqcv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gujrbdhpd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/griqadtdk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gppcnyddn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/ggsuzjamz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gdrgqvpos.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gxxuqbknx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gzknvmzzu.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gallbwzoa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gnvtrvtsg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzgorkjit.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gullxhdna.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ghpkowqsy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gptxrfydq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gsgvxyoes.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gfarwhzfx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gnrzridab.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gkutkxpty.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/ghywtdxev.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gwsfcdvhr.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gnsgkumgx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gdibiibup.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gzappwgjx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gmxjordha.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/glrsshbcx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gnomzwgon.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gpfsosucg.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gtndmeozb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/glyvqvizv.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gjathciwo.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gfhwgduhg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gcoedcyaf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/grjmgdiyw.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gszthxfkl.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/grgbvozdw.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gknigzygb.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gpffffcru.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gbmylplgf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gwplnwwnz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggsirigrt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/ghxnuidur.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gwjdyemne.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gcbebgnoi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gbnwfbkzz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gxvscuzny.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/galxnghqq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gjiysapof.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/glnemkxcq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gfykhdhql.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/glmljvtfu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gtpkoiaxj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gmimygelg.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gjlnjiwlw.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gqqruaknu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gaceevxbo.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gpxmriceu.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gmzeyggks.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnthryuak.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gepvcogch.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gtenpebjx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gynejgdgc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gitxglaok.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gwkeycjdh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gjyjoimav.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gacwqecwx.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gircxjixv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gyjknyfzn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gyvtlakoz.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gafvwucmz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwwhafc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gvpvdtkdq.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/ggcnzialy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gxkcjfvbp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gdnsdwbbq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gbmacgfbj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/glsientiy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gmbavzbnm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gkusrqfsr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/glhgzgjhh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/ghcumuxqy.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gmitajfec.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gkpeydiam.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gnzhbcaqs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gofgisfqp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gkiwhgvjm.sHtML


<!-- 参考信息 -->