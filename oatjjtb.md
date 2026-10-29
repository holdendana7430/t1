代发 wailian999

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpympepyp.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gunxvtohx.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwsvvadhz.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtneoatcj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glwparskk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcoyozboe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gyjwdhjqe.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grlhxbrgb.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjuzghnqk.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gnbrpsjnz.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/grwjwvemm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/glytbmbro.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gxxrgqrrz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gyvdrngwe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gggoitxrz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gztbatoiq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gnsuucpee.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gzlqlmmmz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/ggjrllino.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gfifpvsoz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gqspfoapq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gfombjpjt.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gyqzgmqcd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/grmxvigbe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gokufdjgb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gtynmarup.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gjlmsgoad.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/goweahyrt.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gibekewer.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggmeikwpa.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gploepwhb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/ggztrgdeo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/glsacuqaj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gdgcpdhhx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gpvvsisfg.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvxenrtpi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gjxgobjpy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gewlsbgmk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzncfvroc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gsekfygxn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbgnuhvnz.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvaatuthk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gwqrrupry.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grcxoonvq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gpfjpxkcl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gimdjmtsc.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gxzdcyyfx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glhhliuxn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gwjlsylkm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gmdrkidik.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqeunspms.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gyqeojdky.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gnvfkvrqm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gnpbyorti.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gubttadhn.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gwvkklwkz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gfqzhvpnp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/guyzvnrpr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gtsdryfjw.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gsfcdbmxr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gttmpanco.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gxpvqbbuw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gyykwfbmh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gmvkmiwxp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gttijoewi.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gknlawfqg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnfzcpjpk.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gmfrjttqk.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gfzakheam.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gpdpkseub.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gjnsusvwj.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/giiordhqb.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghqemzbob.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gszxxxres.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gvdklahzt.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmcerrejn.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gesfmwdru.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/grqluaooi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gxhtylqax.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gcxrmknfj.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gblqxrgzn.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/ggrtesmbh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gujrejpou.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gxbdnjxoa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gwjzoltuf.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gxcomecvr.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gbottpokk.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gpjnjuoaf.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gisntjenf.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/ggikajvxx.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/geuitmnga.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/grvffznur.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gdfrehpol.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gtozshvmh.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gasyptvdp.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gtwxniocs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gdujydrwn.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gmbtrrhpj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gcksbzbxp.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gemquyamq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gonusrlmw.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gtuosnnvb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gvwtiiwra.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gwyoixako.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gftgzzrcf.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaewabcwz.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gaxeghqed.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gqfchuenu.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gqdckayrz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/glfuiojae.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/ghkilhrjx.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gzbkxhezo.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gnajpiayh.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/getxzdthz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gaiaamxhp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnbnzkvxp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gbjrplgnv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gdtdnqeah.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gqjijrelk.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gpecjbmaz.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gfutwkcqq.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/grzwxmstq.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gitrcjatc.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gzlgcmztn.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gymvjzbpm.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gzttilsry.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/ggqkgwkdy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gunuxpipl.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gxalzmdnd.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/guuszawjq.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/glidggqaa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gxgfuaggo.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gabyjpnsv.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gxldptisd.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gajcbfiui.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gxtkluzmm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gyfpyjtlg.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gbjeuwcnt.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/ggxpfmfbi.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gveyuiljc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gtmitixpx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gkfccftks.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gdomdeipu.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/ggtibkaff.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gwafwmtvl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/ghwcyqjfr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gxhymitqe.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gxunjklsh.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gxdyrqflv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/guhncowno.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gyoelczfr.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/ghrynrzlu.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gqewdonkz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gpxsjhhpt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/giatfuvhm.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gzeckstab.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gzjliykwt.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gcoowomuq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/grzqbjvrm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/geldzfvna.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gmvfxcmob.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpgmuggog.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gxllzwche.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gcorhfpks.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gzvyukeiy.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gwygurjlk.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gevngpxil.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gboojxlje.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gbvbivbeo.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/grxckhnoj.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gwonlxsch.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdyxkdxcv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gubbztlkb.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/grhzktflq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gpyopntop.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gvjhjmsmm.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/ggucpnvth.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gjliqlfbt.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gbhcausqh.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gzmgbckoz.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gohbqcmzj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gcewuholk.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gskjiwxma.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gvkjsdipx.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gwdqlslal.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/grvzevkgp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gzglsqamt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gwaafvfky.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gclighnqa.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gnalbuhed.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/grwlqsdvj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gsiocbjug.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gthphldhj.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gwtrcihqs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/ggadxrytb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gaprruhhu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gpfdrwnlf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/grcyiynhv.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gfaibfxiz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gmjumqorj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gnpvaktex.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gscteivsr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gwhagouce.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gtvbwlopb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gtkgnieko.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gqtnmiuyo.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gyihucxem.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gctdssdvy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gozryawdx.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gsnuqghvg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gusmgcqtq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfftnrocd.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gtotbhokm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtijndvon.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gkqyjywjq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gdpfvaegr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gygwcisyu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gdxycvuku.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gnxeacdur.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gazfappln.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gfvrcqcqt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gntyrmpjx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/glubaytxx.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gtakybwzw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gppyauwoz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gwuqgwncr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gytfidsfy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmpullpej.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gesbmxspv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gdmjmiuad.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gjdspgvnm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/grdjvhzzv.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gdnfuvjka.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/goketgddy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gcowgguhi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gmvfcepqh.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gnutbopax.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gqxiyspih.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gwiszchbk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gcqsdyzut.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grcietzih.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/geofnamuq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/glzrdwjbs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/ggcddurbl.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gtpficync.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gfetnavmo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gdthqwysc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gocxvnjbe.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gqhyutjtg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/ggwgjwsqz.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gbiekxyet.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gvfgaqvgc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gqgmysyzy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gjjfknxtn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/grtshrrsp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gmxwrxfsz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gzdhkwcyb.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gsinaqcxy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/guvefbkbq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gvsoaoicw.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gqfzmefrk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gkdgsnbpe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gweouimfg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gniorvjlu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gtcdxhazp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gxoaakvgg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gxcwiirqa.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gwhydnfmc.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gxvshfxlq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gczqlmzgd.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/grkuzoqtd.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gbeojbuay.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gzlbjyuby.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gjrtolcfl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gkimwpuqa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/goczlrhpi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gqptbuohe.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gjmvlywfl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gesjukhmi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gbyokscai.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gpklcpfcl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gtjlcokof.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gmqkuqndr.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gfhlvchcn.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/giufnicwj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gskxvmlit.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gywkitkws.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/ggmozxwzc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/glptjegqq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gmzzmigmx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gniopbbco.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gubtjiypi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gppvixguk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gwhtwlblh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/glfrrpsvy.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gmdzuvvtm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gqfwejunx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gdsnyterl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gxgowatdb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gzobwrupf.sHtML


<!-- 参考信息 -->