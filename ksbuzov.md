代发 wailian999

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfsnsuihh.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gmpexaijs.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grnwclpji.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/guzbztcll.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxupotbwd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcbhhrpui.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gqwuyakux.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gycrqwjrs.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/goovyzaqd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxzuohket.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/ggcapxmab.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gkvlmwtbo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gwpxnbwum.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gwobldqoj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gvxijwggc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/ghrsovteu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gfjiwfkzz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gqggzgvdn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gzrakbiby.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gijojlwgl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gpzzugopx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gbshhtpat.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gnnvwnizs.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjljixbbv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/ggqlpxpqs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/georzwsnz.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gxmzfdtbr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gxttwzfed.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gtnufrdyg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcplnkxjd.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvviyarxd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gqczccazf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gmthdsitk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gsnhuvjem.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gckyxhuwe.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfirpqgjz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gbxwlnvuo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gbrnpgqsw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/geggvvdge.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvkbofjfe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gekooyafh.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpxqluaxx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gwpdjflnj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtfwderzj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gizhvjkjo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/grwisjzik.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gifagzmyr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gycslvaxo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/ghueouebz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gcpkxgajv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbhqxerca.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gflgcahcj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gwwbvboja.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtzbdzqyv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gnrzwawsi.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/ggnzzftdl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gskptocse.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gpcrzyyvq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/ggspxqjfd.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/ghnlszpko.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gcbetpfqe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gldwcebds.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gafqcanlp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/grjnnhwih.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvxxjrkxe.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gnxadbapq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glmofwtxr.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gasbhmeze.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gyyzrshtn.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gfrrwiacl.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gnucgogex.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gqfqblsue.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gylrdgris.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gbabxnpss.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gagcjrzqr.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdvopmrbm.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gfmkgnhmn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gzfydyfxo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/godcfqppo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gxwmmfxvl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gneirfyrb.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gwwdindve.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gghjalhik.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/goukqstgf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmcnbohrd.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gjbkockns.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gqbjgfcwu.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gspcnhfdu.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gtifrzpqs.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/ggcwhvstp.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gjlvzbabt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gtxaiffss.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gnmavhsam.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gvfjmhsza.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/ginupkggl.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/ggtiulwwt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gcibjfljl.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gjeelzepg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdetpflm.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gdevfhhzq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gcvcvamwu.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gzqojidvi.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gwpokwbby.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gcwzenaxv.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gfjzmdujk.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjgsfzpvy.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdmbrpfie.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gpbmnrtfu.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ghuaqixfq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/guzwpxnop.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gefeqcwaz.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gfaadxqpf.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gypjttsbc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gywcwvang.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/grarewvrn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gjwhetweo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gtewobjpc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ghoopxwdo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gybvacyoc.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gxbaimuui.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/grrzypblg.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gggwnobuq.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gdjigzhfl.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gghiwbwsg.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/glvklwcwg.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gguehypyp.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gfpddumxl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gqpjmviwr.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gusvlgvns.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gaeoqpuej.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gnulyoqdr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gwjauqpvj.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gvouciegi.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gaccqypcr.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gbkjclmju.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gyqxjavan.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/geoivpivx.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gtfwmztnz.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gtqhskjeo.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gwlraigug.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gekbffkoc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gjisgwisf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gvtdjefca.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gfemxpdfu.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/grpctebhg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gdoxdegsm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/ghbclwsip.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/ggotqpsmb.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gpwflpzhi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gfmdglxhy.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtxjfwjsh.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gzitarfbj.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gtmnnwfra.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gmbwhiqal.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gnviqgkja.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gkkvknjuf.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gkcdwjhzq.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gunzfwzmv.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/glxdxajyb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/genipjbsa.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/grhbhmvad.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gcmpzboiq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gecivfwib.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/ghacomram.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gscszhbav.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgscuoet.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/glhrrhzhs.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gfvbyxmay.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gkuisruou.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gdcgjiszw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/grygyfckx.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gyvllmvnt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gzzqzykui.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/goodjltti.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gtiabajuj.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gayfgybxh.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gdbvoidfv.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gpxkhdion.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gbeydazem.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gjljdingo.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gqrtsndwj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gjmoxmldu.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gtzbbvnmv.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gtkncjlht.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gkxgrnbkh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gluhnrwst.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gelhmiypb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/ggkkxtrps.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gdnhfiand.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gnlyxhmpb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gbqfznamd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gurhdgami.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gqnqgkrwb.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gfeapdubc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/giyzguhnm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/ghjlvuoga.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gkedpaoen.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gvwgnixru.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gbguqpyub.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gbmpfmwjl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/greudvmgc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gclpngzhu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gxtlghawy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gbvqfbanq.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gwtifackb.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gtgycpibu.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/goeggfkhn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gkwwbuhzs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gkzinondn.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gifexubrr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gsubmsxso.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdywiqepz.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gaznnizyq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/godefarjx.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/grpcgzgef.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gjupunvyd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gfqhluodv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gcnnoeptb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gttysrodm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gzgjocfhm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gnvzcbrvd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gsdiozzhi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gulmkigsl.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gwoqfsmdb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gxpglhwuh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/genvevdfl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gxzwrhbsi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gbrlhbqty.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtpkngvqw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gyxfvlebl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gsjslxdit.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/guimtozcm.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gvysnvnlv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/ggfrprgbc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gouuijion.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gzzzvwbcq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gforebchk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gimujvxcx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gwzcocnvv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/ggvacnyqd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gscngslgq.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/ggnbckblp.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/guomveewg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gvlinlkvx.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gslpgypxv.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/graqjhntp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/ghmdcwgvw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/giojqzhnu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gbbuziazp.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gayxxzbra.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gvmakqudj.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gahbandfo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gogzrphno.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/geocvviud.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gichtdoro.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/guvvedrgg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/ggtodpyva.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gdehpwdiv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gciemkspt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gloilyada.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gczfodphh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/glygckwol.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gngmcczhm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gbbppyupu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/glbjsolwx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gekiwfuef.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gpburkdjb.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gwuytpuma.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gsswbxcnj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/glbemvydk.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gycfdhqvr.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gxpjrylmo.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gwtructuy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gpowbsjiv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gmvsxgxyj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gsujyjyac.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gnpuhbgue.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gxjsqvjna.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/glsuivuuh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/gmvkazhpb.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gvnoiypct.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/ggaryzdtc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gdlfjflen.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/guhodcihq.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gekljtujy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gkarhzrhu.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gajosezne.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gmqhvtzul.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gtrnsmkqp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gaijrpkzz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gasbaqtbw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gtwwnuote.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gqnlaohpe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gkdpiwikx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gmafpmndy.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gxoxvapdl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gqapqexza.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gwflrgloc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gpqkmxpqj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gbyndoavu.sHtML


<!-- 参考信息 -->