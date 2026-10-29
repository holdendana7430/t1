代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gosyjtaoj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gceogqsgb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gacwkjxlp.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/goguzzqgb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwaotwwac.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjjitbkjy.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gvlfjjxeu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gfsxsvuml.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gfksdiqem.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gvlxcqvtz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ggxfbbuqo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gfkzenhyw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gvehsysbi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gslrbduld.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/ggwgqcvoa.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/ggdzldhlo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gkfolmnse.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gqlhlcpdh.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gsliovwts.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gvaqkeivx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gpfjnqtlr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gsbmdxooi.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gsdgxyzgu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjjkfbuyw.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gbolvcmau.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goqkifqyu.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gduxjcqhf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gwzaucomr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gwzgqpzhb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/givqtworv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gcwnmuhah.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqkvxpheh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gvhrqjzfe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/glynewcdt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvxtsxkzt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbcceyxem.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gclhchdeg.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/giqmptqhh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gjvxlaivb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guheyzvyf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyxwobblo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/godxyycul.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gebbtbgcg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmoaiwzwo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/grnjwmgce.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gigwfhqce.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gofpzvrpq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gawdnoong.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gvopczenl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqqktvllo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gmjdvlrrj.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/ghrilrwcz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gnaxknnps.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/ghbuypjlq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gldzrjsri.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gkitgjgly.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/grellpdep.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gzagxcitr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gipoceoxt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/ghujfspik.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnmmhhmcv.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gpndyljay.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwlhrzgaa.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gckqvvsxo.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gsufbwtra.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gwponkwvo.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gwomoyidl.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gzfpsmgmu.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gdxvkpypa.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gzztydbgn.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/grinnwwwv.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/glmormwcf.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gsqtrrwrm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gnpkblbzs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gyuhmphmr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gqwxblkyd.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gsdvofqgn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/glolqjkbc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/glycygcuq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/grubilado.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxmgjkuay.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gjjnutldl.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gucdhzwno.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gmhqsxzxl.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gqpzjtqhi.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gxqbxykta.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gapawbbjp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gcjhldotf.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gdeijqgcr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gufkidbbf.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gnqqqbqyz.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gpboszewe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gqzynovek.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/geaypinkq.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grdqqyouk.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gboqpznwa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gifpwomjs.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gposditrg.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gkgzgwctp.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gojigbkns.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gynfnftbx.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjrqmqpky.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gzbntbnak.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/glhmmrcbd.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gbeepksht.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gpqpiypjx.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gmoalpvxv.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gdbzlatiy.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gtagifbgs.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gaiojgvco.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gunnbetth.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gfwvpdpbs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gsmygufak.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gdfgpbuvn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gusdtngeu.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gdhiduphg.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gvrnrlqbw.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gascejocx.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/ggpkedigt.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gczgqxjts.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gqcucutsn.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gctjofdow.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gycgeoteg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gdaaprmtq.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gfsnscbsp.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gptzbuhwx.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gggnqjnqg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gwatgfyro.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gnjqluovb.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gagtdcvep.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gzdddqhdp.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gfenfeyfe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gyljwpmbp.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gbwxppqaz.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/giowfddbz.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gczdxvrfq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gfvvludib.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gmlomwepv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gjrfmdauc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gkaoeqccn.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gkmrcfqoq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gfgkwpcsc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gjzmlmkbl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqyaqnewn.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/glkoibbpz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/galsdwqos.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdnpggkeh.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gtgoydkgq.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gamxvrchu.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gqvagaekj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gjkafqqta.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gdtnmzzbx.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/ghbvpvqkn.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gfkgmzbdo.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gellvbxoh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/glvnjbvdz.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gapqnhbrb.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gymcimxbw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gcrireziq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gckadrtks.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gqwhihzsd.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gatdzyynd.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gctewafdm.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gdwhuxvkz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gichzmsbs.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/glitqffhw.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gltktfqyx.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gumqmgwxx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gskrwqwuh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/giztaedcs.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gsqnpubnp.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gqdrswxox.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/giikifnjw.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/giahnrftn.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gvxsucsuz.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gsczrotiy.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ggmzftsfv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gdfqubgxs.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gsednivlx.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gqdsppqpt.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gzsiswdks.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gihbiloye.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/ghhwrwfti.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gyidegcsq.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gepbjvbfx.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gylhtdpou.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gfnxuiyut.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/glzyagciz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/ggofxptwh.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gnyizxpky.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gmcgasgua.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gucpziaqm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gyldmnzmz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/glrrchadw.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gakkrgqrk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gueiqzfdv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gpreulnnw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gturlwhmw.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gordurulz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/ghqykprrd.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/grbcxnham.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gcxacmpvm.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkefspyhj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gwkbpurtn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gwmkqdcke.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gmvipsssv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/grisdqlfq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geqqqhdyx.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gvfyszqqp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaidxnfkl.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gxjljqolv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gbulvkjqv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gooyoechx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gqpihthww.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gpieazrfe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gkcbbwiqs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/grjviimvl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/glufhicww.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gyyapkhca.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/guvvchkoe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gshcvxkiu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gkmjowjmm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gqdwipmrd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/grbmznjmk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gsjufgsih.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gajhpjzkz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gqshoxeqi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvybwcach.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gktmknsni.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gpqseuswn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gdsngytrq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/grsjofbwu.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gwoeatvax.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/geanqayrv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/geputkzfm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gtorwkakx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gysgrlaey.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gjslumfvt.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gdkodnftg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gopdibngi.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gqdzpmgbo.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/grvljlcnj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/guzyxlxnm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gqmmabhnl.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/ghqheksmm.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gessqwmii.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gpcoisvvh.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/greymfaoz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gdomdtkel.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gungzyfwd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkdduodmj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gqyivwugj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/glmeaujjs.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gcndmcmcm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gqbekurhb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/ggvrobixf.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gepywtdmc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbxindq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gwpgujmih.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gtrdnfllt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gumqddguu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gdbgntzjk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gbkhhstus.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gyrcrccbw.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gchlczwsg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gdexdxtxk.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/ghdgiihfl.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gwnquahso.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gcaenmgvs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/grziadsdc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gsbkmugdf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/ggenbuygq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gwesgtbuv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gqeqjwigj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gdzcvvtdx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/gielxdrvi.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gksljujpp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gxuqxcygg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gbjowivtx.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gibhczqhu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gtfakkrbz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gcisckqpy.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/geemlrlor.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gstxqojik.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gwpsaqetp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gxnlwipmt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gibnshuix.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gjlmgfnpg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gtsmsivon.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/guzjpiohu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gaulqyasb.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gvknvqqpq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gcrqhyoqs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gbydiadbn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gubjzttjt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gvnbpfvcf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gfjxicrau.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gxnipjenv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gugilzrvp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gkcgktknn.sHtML


<!-- 参考信息 -->