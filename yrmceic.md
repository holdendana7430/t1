代发 wailian999

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtjercmew.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkipmhmta.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gpfqjvoku.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gngiexjfx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gtfolysyc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gohfkhapl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gxvfwiyqa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gtcnkmeep.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/ggohaurkc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gcqeifmho.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/ghpgrbeay.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gflnaffbh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gnmonbazx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/giicpzntz.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gxedfksux.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gyjviovru.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gbwricjxc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gxctvlfxz.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gudwrqnnw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/glejjodoa.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gaulbrgoo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvfsvdjtn.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gexiawxfc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/ggtodoqee.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gzyyzysvt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gyvsejxgd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/givpuocvh.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxyzpltpl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gtkygvpiq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/giyiwajag.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsvzaisnl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghnkperoo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggaauoxiv.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxlbzcacr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gkwodonsb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxfsjdtqy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkodncnue.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/giiudkksj.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gidjynfmc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gztwowboh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggjuwugjy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gxidpefky.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gksryevbt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gtmalkumh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gpricanyi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxttkizoy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gwjxgwjvh.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gohlbmply.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gldngsvou.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gtgygkaqx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gewjuwlbs.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gzhcgztjh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gukpcjopq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gifegvtqr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gyvrzhrkl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gcpusuofe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gccafcsse.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/greqrqbne.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giiyrxzmv.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gxjmvbjbk.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gqktscfqw.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmylyhtcn.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gcgjodmuj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/ghypdhgha.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gayzlxiui.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gggwzchrz.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/guqivrgmq.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggocqliui.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gptmbdxxz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gphchtdun.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gpjomdxwb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gkmmetwmc.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gpjukqydt.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gxaicfvzj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gqoulrnkb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gzguvazsc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gqiuvpwqt.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gxpjoekto.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gnzajijcu.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gwstvuege.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gsfunbayi.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gyljaefoc.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gmffvlzvd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gielwaxet.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gsqbwxghz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gfnbfwduv.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/guxirhsug.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gflwxkmwb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gcwaqitzb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gofyfubwu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwjvnvlog.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggoumxtnc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/grsfncjos.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gimcfgfbc.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gxcxqanjt.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gmyvwkkob.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gmpyapvsb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbpuakzcx.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gsonnyhgb.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/genxmakkf.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsryeaeje.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gcaynrsja.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gpurdejua.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gxypwopoe.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gdhtcikcz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gpqqfpiit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gmirnvyzn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gawptzfcv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gjenbpexl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gsmxkntmr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gwbqnkhea.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gzzdubpez.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gwryhqosx.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/glukkyjem.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gjblecchj.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gzzqusvzy.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gakamevgj.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gkywzbokl.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gnkofachb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gmwofmfvt.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gvcfuiuhp.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/grakjsydn.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gsuxvoobz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gmzulyehk.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdxtfytkc.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gjjajrnwr.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gqunznytn.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gidlwgwys.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gfzmjgqsw.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gmslmsasy.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gbhrmewfo.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gkswplttt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gguwtqedw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gcumilprw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/glwgbyobd.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gdsvgpnou.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/glrnpznbj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gxmpmudxa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gvvkdagej.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gwitfshxc.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/grhxmytba.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gghpmdgbf.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gicndfwhq.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gzcnreptn.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gnzpsceij.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gngxzzacm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gwfugovxp.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/guubvgtyz.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gmkddtmgw.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/grbyfxnfq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gjkptwibn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/govlixveu.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gfwouldpv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gturavulm.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gmuabeokt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/ggerzcren.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gattofrpq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gaidvxdad.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gljfcdxin.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/goytbzawe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gccpgwqcx.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gwavptbru.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gkssludzj.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gfsiivtgi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gpbitygsi.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggbtlntqa.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gdebuscvq.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gelbcwhde.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gusvfuwub.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gsxupbjrp.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gaeffecii.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gdfkjlexo.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gucfcurpy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gwzvcofnl.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gociilcut.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gtlljnbhp.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gomcuvtgf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gqutwweqp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gmkqpoijf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/glviyjgox.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gzwbotivg.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gpnxnrrwl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gxnmredxz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gsdwlxgbf.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gnljyaabl.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gscwtmvze.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gxawtymfn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gtnmhcogp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gdihqxfii.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gixuerudw.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gvjvxkhrm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gqlwtirpn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/glzjzfsav.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gqdjktqud.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/guklrjcrf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gsenttsmg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gqslpspkn.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/glyrkbnyq.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gdzdiqigc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gdlxcwsiw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gvjrkaprl.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/grkvpqffk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gpcwmtldk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqdojsuwz.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gvifuuypc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gekllctvy.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gxljvczve.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gptlsqusb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gxexmpede.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gwrghpfik.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwjzfqchg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gmhuxfchq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gtgtgkncd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gktkufubl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gsuxojetu.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gxpltejhp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gaasskzzd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxvlfmtxr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/guesbyiho.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gowkaczct.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/golakadvp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gxfurmrne.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gtdmjrrym.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gajhlaqcu.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gdeilnqve.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gdanrtrfg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/grblgkdlw.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ggqfcdjkv.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gnjamdyvf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gwdpfaaud.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gjnllriko.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/ggydzabzo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gylywkrbx.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gkswadumv.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gooqzjjcw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gzyytrwoi.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gjigmvtmt.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gdkavwzib.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gkhdeqdyk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gzkpnuzom.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gjdgteqpd.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gottmcrxd.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/grggizhsa.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gratklvyu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gyapcrmdz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gdejmpzqe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/glecekhkb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gbaqkjypg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gnpbgesgn.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gzrzkjgrd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gojwsqbtt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gpvasfavc.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gbtocahkt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gdyradivu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gprwskhgs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gqmoldwol.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/glfdwmsfc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/glgkwuuhs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gdnqjtljp.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gyuzochof.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gdmqbnizz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gfcakokrr.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gnrnnkoeb.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpsjstgak.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gllzlynki.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gfzokndne.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/ghvqicnye.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gruzxkvpu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gbpjinnwa.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gwpoiroeg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/goxprdgun.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gxofscurn.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gttqormti.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gwfgorqfb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/guveqhklz.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gefoqpcnu.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gbnnupxzk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gxeqpvobw.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gxgkfvbfc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/geqkciijg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gzvbecuzy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gmzbxveie.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gesmnxhfn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gsxufuzie.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gkayrvhqr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gnpsqsggv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gvtkxzagy.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gadexpohr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gwvdqnosf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gqycccfjz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gwafsahoo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gexgppqyc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gwqjcufqm.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gsvewbsat.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gbgwhgnwn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqtudrlbf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glcuyoagi.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/guhzpyfti.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnwjebxmu.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gunnoqevz.sHtML


<!-- 参考信息 -->