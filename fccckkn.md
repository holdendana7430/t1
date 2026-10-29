代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gdlespxhh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gxzslkivi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gfoyjbutm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gmbvjkjwn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gkzoayuqp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/glyveprec.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gjklfglry.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gggoqoiod.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/goxdyvkyw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gjnrcgwvc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gvryjenxp.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gaihrhkxq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/ghfmadhtj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gyxatuwve.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gingwultf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gbfrebtpb.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gtnuncnwo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqsledzfz.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gsqwbzmng.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gbnvbwjin.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gstzabhva.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/giismowfs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gihpzmnvk.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcptotfpq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/ghppnyxax.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gkpsrhmgq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfvswmmqd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gckkgnqsb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gsnzxvgaq.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwhbntby.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/ggnruejhq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkccnqucg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ginhbziqn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gavdbrhwz.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gtpawthdm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ggcmvpscm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gglvssoak.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gkgwsilxp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtpjdwblv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gdilaaquz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gbxxyvzhs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gqimsnifw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gnfhakqer.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/goiagxupv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gfzwpfdct.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gyokourko.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gwuxvnisr.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/ggomvvsgd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gvotqwijg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gqrmehdfs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gvgajlpnw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gwkudlrtk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkaiosdfk.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/grzzgbvnr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfrjfnlbt.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gompezwjd.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gfcqsaovr.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gwqycmtox.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gyjefjoez.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gfznqxjdo.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gzhgomlqz.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gepsjqrmg.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gqucsmlvf.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gsyuqtjhh.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gcpshpuyc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gqljicqlt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcsvxgnpg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqksilpsm.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gaubxhkqc.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gndumvezo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gaxmnbgvo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/glfuwfgnv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gfdytgptc.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gscyyhevm.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/ggshqplav.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/goanpsqct.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/guhedgqar.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gwncbojpo.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/guroicdpz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gtdnwrmwy.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gxdvmafwf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/glyfsvrxg.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gfrpjdyuo.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gnzukqjpm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gkhteinip.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gtvwhxcja.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gdtlskcei.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gwlqppuxz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/glnqatpyc.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gguugyqev.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gnbijtjag.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gcrrywwwl.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gwwsmyfjp.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gildwyzsm.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gcjnoafjq.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gycursmpa.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gcbkrdcze.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gyrwxzgwa.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gvunxgxgj.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gjlxkqtui.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/ggfukcerg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gezcndcyw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gnifzgqcz.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gqtgcalxm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtfgorsyv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gcpbhlswq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gaqoifbzi.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/geuxccrsa.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/govjzakaf.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gkpvfytih.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/glfvpqoak.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gzdzybiin.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gapbxfucj.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ghkddqyso.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gaaoxjmsm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/glmjublru.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gqfnccxqy.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gpybzqcks.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gishaymig.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gnklgkbuf.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gzwpmzvjg.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gvvobtdxt.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/grcmzhucn.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gpxfpuijm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gqkzwjrff.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/guysajfbs.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gogkklaob.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/goojaneuz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gxwqezlng.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gcjjrsrfn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gmyerehvd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gainayjet.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gytnmwlgw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gwvmkrqxl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gckszgpsu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gbqbuouet.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gztfftrtv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gsgqmzfpz.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gvjpxoxaa.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gmqwnnhwh.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gvdlrpazi.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gzgofimzi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gmrhzlavr.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gpkolqzcy.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gdvqoclph.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gxmemlyua.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gehadngzn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gpnaboueh.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gmflesyzg.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gblrfirif.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gcdvqgqum.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/geprdxjlu.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gppzrljhn.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gythtfmlh.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/giutiylmy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gkuzyydtc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpgrdjrht.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gzgdaxorr.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gtflrwesz.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gnvqexdre.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gblcpdkdq.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gywvqmuex.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gczxmdyml.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gachkezor.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/geaogqstv.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gctjqriwp.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gjwszfudw.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmzsqbdaj.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gfsgrokhd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/ghthoybob.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/grazamphz.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/ggomahzdj.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gdszaskrf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gulewcueq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gwfszcheo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gdmaaervt.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gipdxnzab.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gaplyehbk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gosaxscca.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gghyfibll.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/grfhgodyv.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gvmwquloy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gexmxvpto.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gwyfchuvk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gikpolzfi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gtmzydxju.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/ggvcdibpi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/grysrtelm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gxycdpabo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gadwqbiqc.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gijsuwbkw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gddhqvhmb.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gqnanhysq.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gugesrqpz.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gxsmxwhad.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gmpftcfoo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gmbnvvtaj.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gzkpteyqn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gvtasbrpm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glykvtvsi.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gtdbsppkr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grwpqobtt.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gcqnqkgll.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gtwhyuwdi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gvehapzit.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gmxrrkhls.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gkdwtpyjz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gacptfwya.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/ggfnxpcou.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/guordbhyo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gutucbhlx.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gmbvrdxxg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gekhszkjs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gashqstyq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gyvayqeto.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ggqpjecqa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggdengrwd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gbuucevti.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gmzthvlkt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gqdstseyq.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gxclgsnnz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gjledcnrm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/giszyjqzf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gssjxvpsb.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gsgpaiytf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gqvjydnyy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gadmavnrg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gpzsnaaxa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gownqskqg.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gfsbnwace.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gnhaampgt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gewhtvbrg.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzxrtsobz.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gwjpzipin.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/grdeehoky.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gwehxrrym.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gbuvrrkgu.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gyborbiff.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gydjljutx.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/guqfqhmvg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbpeitaay.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gckqicsnk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gbuafhyqa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gyckdkqht.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gouqdxgsk.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gbqjunhzu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvjvsrphy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gyakgwrdn.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gblzyhqyg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gagsmdkdo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/garwwuaqv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gteuuxkub.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gegljihpw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gxbfkujbw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gxllohaoj.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/ghayqxwcq.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gcgotycvy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gwaffrffj.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gdqpifvrc.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/goolfagqk.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxagzplun.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gvlpjsklw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gajuxlwbb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gkyddwvsv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gomlouarx.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/ghowkzpcr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gqfbvvaog.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/guyjkuiwr.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gdwyzdryb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/ghklfigmq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gcibnhdgp.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gxcinqsot.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gbdqiyngl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gupqoycuz.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gglvimaxg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gyoashuui.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gznoeqljh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gvyhfbyjk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gqezaruom.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gtxteuech.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gmgireqwf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gemdzecnn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/ggxxtcevv.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gdnojjwjf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gruvbanpj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gwewtcnak.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gigpuykub.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gpbijywox.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/geibahmwz.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gbzkldmry.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/geadbkjan.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gluxqpevd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grfrgvfqu.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gnobiuygo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfyxnxlbg.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/ggeuqkyoy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gzobutysq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/goefuqjxx.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gfertdeok.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gbopyfzoz.sHtML


<!-- 参考信息 -->