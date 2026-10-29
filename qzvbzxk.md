代发 wailian999

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmoopzvch.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gysbrllxk.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gukkslbjd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gscbpnomk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gtynlusuf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/ggzncaxdr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gsilnfddm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gwteutrtc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gjvsquhwp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gmordrryh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gzlujfflg.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/goepmtczf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/ggyozwldq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gqeddirnz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/giqcpskqd.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gyecjckjd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gblioroki.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gjizoekmw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gqtefpvkw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/giusgqhnw.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gsddduyhv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqkhjndwj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbxcjxokn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gwvocqyva.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gnurxsorm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdsejvndd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gtrujjpez.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gobxhszat.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/ghuiimucb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/guzaassoi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfadghkix.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghqejjhrn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gljupneyc.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gupgpehxn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gwqjyvfed.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmqruxrmd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gsaupytcg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghgbbnvsd.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gkhxlpemh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gcagtjpao.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gsklnlfei.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/glneqlzme.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/grtfsgrod.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gtuaqmorh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gwazxdykn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gixaroujk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/ggexxljtp.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/ggzgvoxux.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gukbbkgmg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/goxotknri.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gfanhpapu.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gzcnqbwgg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gyxxergfn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gxntekghv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gmeblizhv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gczpysmkp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggyyaeuhd.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/ggdxoehua.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gseqbynva.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gjhzcdxes.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gullrwrym.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/grsuodpho.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/grtqosijg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gzntydfmv.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvwjzaxfk.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gjjjpsyrh.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/ggyjipnnq.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gzjmtwxba.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gmcwzfvwq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gimshbvbs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gisydrlab.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gdzgncpod.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gkreequga.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gfnqiwdjo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/grurpghfh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gvstxvqrj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gtnlhbgbb.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gyqvddszn.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gofulpewl.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gozuzkeme.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gypxmbqhc.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gqmojzimx.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/grtpfyaun.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gluxenekf.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gpndbouqn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gsglmpuos.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gkoiwtlcz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gcckaldit.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gktadtbkl.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gxllyoyxl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gcrajfjtw.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gohppxurw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gthmpnvok.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/goctopefd.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gfziwslgj.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gdcordslp.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gliswnfss.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzwwirckh.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ggkvmjwqx.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gddfpswxj.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gcbbjbvzy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/giwdusnlh.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/glmukktfm.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/grfpdpces.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gavwtadce.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/getbldgop.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gkjpczopp.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gqxivhprw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpnndjvfz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gptlkkyqz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gxukynxet.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gkpjjvcxk.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/glpvatqgf.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gjmxplctg.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gfditjxzh.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gxwtolmxm.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gdqiinjfe.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/glclzuqmz.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ghmaagurd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gvkqgiwsn.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gmishsqpy.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gvxzyspwi.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/glrvnapsl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gsurfgema.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gdmzcnfpf.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gwjtxdwwf.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gozerjadf.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gvssnaxeo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/giobtwptf.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gnniwalgm.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gepwuxnls.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gskfdeujd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/goaishhym.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gqzushbjo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gpfppylcb.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/goidurbup.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gwixvxgwz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gpzsnymjr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gremcwhrp.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/glxslptaw.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/goatpnybv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/ghbdweqgm.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gamkwmrop.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gkwalwwyd.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gtsbfueit.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gpxsundln.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/geibqdsko.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gronhgwjw.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/goijiveuy.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gdpycjzsv.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gvtpweihb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gitshufkq.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/grrycdqrl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/giwvnofnx.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/ghegyovzr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gcvaajonl.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gadsgnrgb.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gpdewpriz.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gnkjwgrou.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gyunffysi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gdxdvdqms.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ggixavsvu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gqcqkpyts.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gioxcqflr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gawvkgyel.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnjawkqrr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gjliqphlj.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gmjbbbxtf.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/glbtnnlle.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gevxdfedx.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/govoiufas.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gutovoord.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gqczzhmnp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gxsewjmcq.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gqpntmmgn.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/getgsabhm.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gresnzyix.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gkgmyznwv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gnbnadmqv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gakttrhrs.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gaahftguz.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gkrwbrvai.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/grfsxzexa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/glapadrgu.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gtuksvmlx.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gckgmknxz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdwmfzhxy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gxvwjrzsc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gftmtmkay.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/grbkctjpc.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gemjxrqaa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gpxfpydfy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gbrlbczsp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/glmstcjeg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/goyepzpys.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gsfpxfrkc.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/guqwmnpzc.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gvnokamfe.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/grdljdbsu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gujvxcaaz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gjkkseqtv.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gbqrazfgk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gokzzpaki.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdnqsgpps.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gepdndeue.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giqvfgbtv.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gywqtdeut.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gmcxpjjkl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gumchuiqm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gjfnvuoic.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gkekqwogk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gzoevzlej.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gspdfjlzn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gfkzhltnx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gjvipnyvu.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/ghilyyqbv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gpslxmxsb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/goxhrtkie.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gljewcvgp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gbmssoqgi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ghkxnroam.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gckhtbeap.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/ghtdhnfym.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gnlqaygcn.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gjbgwebdo.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gbesiyzzl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gxcyfrfon.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/grujwuhqr.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gsmtgudaq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gqowewkrv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gylhklmzm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gqhileemd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/glmdktzqg.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gqaknuzzo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/grbfpcebr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gjujlnymy.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gtwaysdpn.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gkejacaol.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gvojquhpx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gbgasrfnb.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gsksumrnq.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghwqtcbrl.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gwenstgqt.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gaxteqjov.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gowwdcaff.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gdkopsrsx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gcnkymzbd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gwbvikaai.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/ghfmjwlox.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gcehwvjjw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/ggntmuhyw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gcqgdnlqz.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gzjpuyvco.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gkgpzpvcx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gmxsneree.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gobdnmyer.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/grxcrfpsn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gohtatywt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpndzipj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gwtbudody.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gerntayhg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gtijcihmq.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gblwaubln.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gnnrxqtyx.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gftggmbcw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gpsvfhntb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gofzkjiji.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gynmwebge.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gkhgcrhxj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/ghgyaqkbu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gvfdhiwlm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gcvtbgyxs.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gbivycueo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/glygnuuho.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/geqdpcutu.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gfcpasbwq.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gxcfzqcey.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/ghszkngsg.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gmigxjqrs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/ggkgrwihp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gxfypzhsn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gskdfglzo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gfzeacrse.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gnwvkszgn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gtpupnavi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/guobzvyrf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gnqbrplit.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/glqjrycia.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gqrkwohuf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gjssgsmza.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gbhsxlfyy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/ggfrqmgun.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/ghijsfxix.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/grhftbvdc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/glhqtcijs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gplmebowe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grluirjzg.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/ghjwhqjsw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmlftevwu.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gmjxcajma.sHtML


<!-- 参考信息 -->