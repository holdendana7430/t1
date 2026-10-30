代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/giulbalcp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghwagzbef.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gxkrtztcw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gebxhcpux.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gghfqemnt.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gveyrslqr.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gydlgkbsm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gvnrcilso.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gstltwtbb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gjytoymam.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gtmwmktfl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gzpzkbavm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gpmikvkjo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gnuafoydm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gsgupkzjg.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/giptcuvqo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gnmcltorf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gshpxcxox.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gmmyuchoj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gefdpwxyf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gkllsrplu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gmjwbdpfb.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gbkveyeyv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gbfpybhpk.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gohixanbq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcjmrxvvu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/geijlyucy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/goijbnhri.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/guxcnfaru.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gbilzwqmm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gbusqupfx.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtrrynmkr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gfapnjbql.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gqoctxica.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gsqosgwom.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjrtindxf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gpwcfngde.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmprfyjyg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gfwjyqdxj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/grdgrousj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gpzhmytqz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggijjydcx.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/giqqqbuum.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/glorqikyo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gbelageug.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grbmmzund.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/guignouby.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gqtyphviy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gyolzchru.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdpysgsjl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/glxubvkhe.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gyhsefurq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gvqsfbggc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gvfgpskbl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gbwdotzld.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/geqmxicqd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gpilkcxrz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gnitvahsc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/ghvieshrb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gsgktywqj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfqqqetdc.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gebxuhnje.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guuadcmps.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gapuouhlf.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gvtyrhqpt.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gujamyxvs.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gkegnpmpi.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gtuveohnu.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gcciytbfk.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gzcgajepp.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gwqtnykcl.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gocryqknv.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gmexpoejy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gzsrjwckg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gmdrfbvxs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gpqpmybhz.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gkzcmrzcq.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gstjplrcf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/golpgqyzf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gcvxsqgby.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gqlzadhbj.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gkvbzlesv.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gvtvnkxhs.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/ggfkjhxzr.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gpekhiahe.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gcjscpzdf.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/glprxslxu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gyhzbjiht.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gfkqarjuc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gsiwqdjne.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gfqynibhq.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gszemxfko.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjdnuxisp.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjobvpuml.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggxlzxkku.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gnkyhszwj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gbdtoqfdl.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/glauagysl.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gwfrcgxqg.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gbnokxlpw.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gssuuxewr.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/giycjsagi.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gyhtowgjt.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gajbjwyxr.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxccyqggj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gbitpftxu.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gkftcpvkp.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/goowpmlla.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/glutifrtk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gkcycqhlp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gymuylcpo.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gglmklsmg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gzsykbcds.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gglaevzot.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/ggznymcen.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gpixsjdhd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gqgldyxkt.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gqxfdszmn.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gaogmtafy.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gudssndhf.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gxmnxxxbw.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gltwmjcmm.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gewfpwwuz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gduqzawwp.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gbtnyjvwx.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gtbzfufrf.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gjqldvgca.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gxubocbwk.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gorvnmdis.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gstyssiab.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/glngydxpl.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/grdmclhcy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gqxsmerjy.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/ggrrjrxel.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/ggllqaukz.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gdfagtcns.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gfjauvhol.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gbsksrrab.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gdyzkwyox.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/ggmxpdjob.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gnsgwrgwi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gzyxpbeam.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gurhmpcgp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gpjztwxyg.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gjedtrbjj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/ggxohcqak.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gekpwsxdo.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/glwbsctam.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gdseeszqi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gnaxfdaxs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gglcamicm.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/goudzutbo.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gffcqzafu.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gtkbvvhok.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gbpphyfvh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/geavekmzl.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gzrscohla.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/ggquukuou.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gplrovyqv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gfpgdtjai.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gshxozmes.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/grqnxydje.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnnwqztrk.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/ggqeiamrh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gnsbarkep.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpzzkcvvd.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/giyrwsokm.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvowlfmmd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gxrfbyald.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/grtktqtus.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gmvulobhx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/glxyznscc.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gtmpdtaek.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ghqfakbvr.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gukrbwhss.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gmtnlqvyh.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/glddqfoxu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/galtiuumq.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gowvxohto.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gezhjtehp.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/guyhsjokw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gewuejutb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/giggwdvou.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gbavekoca.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/grewktmgs.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gzpzsmrxl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gdahbvmhi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gstrfrlvw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gbfzbwxgp.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gxxzikvph.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gmdfvndhi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/ghbsydwrv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gjcuahfuu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gbxabfhqf.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gqiojhtly.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/ghuqvuqbl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gskkhxobg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gfdjzbzti.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gjagabepk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gunbplnqr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gtpijidaf.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gdamcobqn.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gpbobbyor.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gnkzttxbb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gkdyncjit.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gqvrjbmcw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/grrcmgbsw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzqqsspyg.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/ghfyhgujn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gszlgbxoj.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gaqmlpeut.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gfrohooor.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/glwntsrre.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gygeedsyz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gecrjztrp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gxrjafuvl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gwjbayrkc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gqdrqyypr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gkwyboqnj.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gbxioqdpb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/ghjezljvx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/geqgblhmq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gxruffxft.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gdmcadnrt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjbocpzsc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gvvbywkqp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gbhfporrp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvjwsctiq.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/guuuqbvcm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/ghlodwoff.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gmwzgnxja.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gewoewyyd.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gpqorlweh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gglnhnivm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/giuklwllp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gjjsgxzzk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gpxuvnclg.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gecqwtbmh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/ggfibnrly.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/grycdtdkl.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gajdsalas.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/glktokxgh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/ghjujlhun.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/grekzmsat.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gwjdaevze.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gjnqwcyqh.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gdttxaego.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gmkibkbts.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/grqznqtip.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gjlptgjsk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gpstocgvi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gwircybnr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gvknddgcm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gyfjrrvzu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gignzbzsq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gmnrswwac.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/ghipomyhj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gcbwjczvm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gckqbmjpm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gvzvtmagl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/guugydhct.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/glljaftlv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/govcuedwg.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gyfaaypzc.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gttnmptnf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gxbjubogp.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gfbtsklcm.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gfaxvmair.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gawwbklne.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gwpugevdu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gxvezivqd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gujidgyhw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gxrwquraw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gitkyuhqd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gtkqhswxm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gkhzxtpbj.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gunsipqny.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/glfdlcvhl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gelfxadsj.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gxxuldwxx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gxlpryoko.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gcjftzwoj.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gbzudagdo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gkbbcrkly.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gntrmvvlt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gtgldpocl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gbgieunui.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gspoepdaw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/ggikwfflk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gzmucpegz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gotfirudl.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gemsvbjjk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/ggujavtiu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gocjmgzdo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gicezxgac.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gmssyuikb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gbbxbsbjh.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gxvhpjgrj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gqddaiwyu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gercculjp.sHtML


<!-- 参考信息 -->