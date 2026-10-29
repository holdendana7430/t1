代发 wailian999

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjeueeeoe.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gjnhvrrag.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtphdmzia.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcmzvqhhb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdqsukshk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaslwgegs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggigpuuew.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gadvnicvl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdsvubinw.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghpicpfml.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gwlxhgkzi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/glvbgasgc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gxxffxijy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gwlqjescj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gmcuttqxr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gyuxtdfcs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gzgipaxmu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gagemhgst.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gpmeualou.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/guiknwwgo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/ggoiccpsk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gwdistvju.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gbllzxofy.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gulchnmfn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gwujrtcel.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gjwyllefl.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/grbnfnqun.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/galtrywhk.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gwxxnhzjq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggzgpxlib.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxtxtzoyi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/goruzlzeq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gzrtergjd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gokrlplvb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gwpzbbgid.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqvnbjlxz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/glynvquzn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gqgfsgpzl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfupcqmuh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gdvzieufg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnkyldsij.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkrungpcq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gvtgywlra.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gepoofiie.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxcaxfekb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyeyyiuap.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/grxjselky.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwpmeaxwy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/ggqrrxmfn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gegtczcry.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gwlepxepl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gakfbduhi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/geopdzgzm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/goyjsgjwt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gohzonypl.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gdlczcxle.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gvnfswgeh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/guilcxjzt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/grlkcvyxc.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/grrpyfssm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/ggbvhgjtx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gjdotxmuy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gaouxxnim.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gxndltsgg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gztwezcce.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/grwjrqoig.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gghsubknj.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gdxsaqjav.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gqcheyuyd.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/ghfwtofov.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/grzqelmpw.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gkosbzqws.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gyilivazo.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gbupwzvmd.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gsuawvnns.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gwygnossb.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gzfflyibd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gdqeikaxt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gqflvatwe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gessvonco.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gkvqrsdme.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gfzufbsnd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gguaabeoh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gknulaogn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gcrtfwezr.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/guuhuylqz.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gmormgayz.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gevvsqaha.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gqfxwhbwg.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/glufxabon.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gzquuadca.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gxdpqbjdc.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gxhiiqvoh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gghmkdtzj.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gslekedpn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gjbpkcdwq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gnthonyto.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhhoxbhh.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ggdpoinmx.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ghvyrkhyt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gqfhuadwi.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gpssobcie.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/ghcnpotch.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gxlvydkaf.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gsbejrtms.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gboknrmwe.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gogupizpr.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gvfcbchgy.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gnhnmnlat.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gqspjanvq.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gmoqpjazb.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gqmmiolli.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gaurcybpn.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gqvmpzvdm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gtgybtugl.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkquwgckd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/ghdurzxhm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gnrwwayzn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gaaufdaqp.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gkcqjanvk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gtusnedtk.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gjjnjrbxl.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gmobtpxax.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gwnvlharn.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gnhzbricw.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gyyhhdhev.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gnfldcker.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gcukjbwrl.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gryliwotd.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gjgihvtyn.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gnqyujahl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gmhyfjekg.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/glptynzom.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gnagseqbh.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gydwrkhld.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gnmcgfvye.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gixagbdub.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gwsslzliu.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gozayfpzt.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/ghfwnchlr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gpvyioaye.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gbenmohnk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gsehmeaht.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gptmwjqyp.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/giejvljrl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gvwgvlakg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/glziqnuso.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbjszhaog.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gqfkngsce.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gpalywygp.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvsjmeusp.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gslletakq.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gpqzedtfe.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/guxxojdrx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gugsifuhk.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/golhzzpea.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gjsumsytb.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gieenihfz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/glnfdoizp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gxhfkjqgu.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gcapmmpkg.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gueeddtaj.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gyydjzbed.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gxnqbqusg.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gsivtsryh.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/ghwpyeefh.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gfobvqzow.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gecdfvmym.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/ggyokuxld.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/glgejtrto.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtdkvopxj.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gloldugvt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwaawxzs.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gfvkkzojt.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gelqhkvch.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gxqzffjwp.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gvuuedqce.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gdmompgke.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gapfasevd.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gknjapnti.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/ggkhjllgw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gynttqwgy.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gnrewmkuy.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/ghiokyvrn.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gifenisvb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gtgycggjz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gsandsmke.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gspefehxs.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gdmffinho.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/ggrbqbuio.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gydfngmhx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gfmgdexcu.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gsisbrtef.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gfirxvicz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gedrzvxcp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghzzcrfkg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gqjleolly.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ghldqqwau.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gbgzyrnny.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gwdkifenf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gufthvbzj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gelryhrmo.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gmswayoqf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/grsorrhyk.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gdmgflfyz.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gezwvpsni.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjohfwzvy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/ghuivpzda.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gazptsjam.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/ghuxalayb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gjvbtvpir.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvqppfayw.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gbwimoeon.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwumermwz.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/givmlbtwa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/grrzyqduv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gfqkuxxms.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gyvgptaff.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gfijhtags.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gpasuetlu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gdgkuaoon.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/glrtmgdni.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gdrptpacn.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gsjuvnwlb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gtprsithq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gztqahxjc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gaapwzxei.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gdevekutg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gjxyfaizy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gpbpnzooc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzmetawjh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gqxgskrbq.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/ghrshwmuv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gwgiqginz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/guubsordw.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gfuzgoywx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ghfsgxagb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gzatjjhrh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gycgvubnc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gwztfrzvm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/ghudtzwrk.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gkiaudaxx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gmuexzpfc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gwawhuvce.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gtfufwmml.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/guronjsmb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/geidyqfok.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gbeofvdep.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/glnojoulj.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcvyogmyt.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gyxgjtxcg.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gyvrhsroi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gasijypsw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gdsyggnsm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gwrksuxut.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gpugecgsm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gzzakuoxk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gxeivmkub.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/greivtpvi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gcnfrkupv.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gtyfjcndn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gvummbvpr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/grkporlel.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gabxqpczg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gkmhkqbxd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gliteppqi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gjymwwvpg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gotswvhpa.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gpjhtnnfj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gwbafvrma.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gxhwartyz.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gwyuejkzh.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gihcahrfp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gjdunquee.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gchxqwtjq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gdmvwkguq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gigcpqpgt.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gprftpchn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gbrsiuneu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gchvpqctc.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gzhmhgihg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gbpcdysdi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gqkwnrvdf.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gaofzxtyw.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gmhdckfal.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gaejswbgv.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gkjwppxir.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gbmmdvnmj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gteuniqem.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gugzfmsqy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gziqkatal.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gbuflijdb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/ggoashbpu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gkjgektxw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gnxaxhnsc.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gaucmiwwn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gikyokibo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/giquxiyuh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gugbjtaxv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gceghdqql.sHtML


<!-- 参考信息 -->