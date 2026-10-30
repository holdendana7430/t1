代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gmuhqkvfu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gyepmpnov.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gyzrvtkds.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/ghmgmbhtq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gowsvltxl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gnhrnxeuk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gcprkeoyf.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gmaoxcifq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gvgfaxenj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gxofzvvnr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gyhyyiclz.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gscmzijrh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gohrftani.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gvehsgbtj.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gvizhzjnp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqlwxcbql.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gehxyzptw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwidzbudw.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmfoztgfy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/grxwrsgfy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gjxqyfoqt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gdthnmrmq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gndgllquv.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/givyknjwx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/guiwluokl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gesfpceot.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzoyoufxc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gsnqngmpk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkdezonlf.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/goqtgmfla.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gkapkjnda.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfwahugku.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gmnjeyncg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grrlfxssy.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gooqjxnze.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfdrrxryz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gcojaumuy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gapsomebd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdeskqzrw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gfqxultna.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/grddiqxmz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtwapajof.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gifhhdair.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gptcyemvb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/giewazopw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/goejlnybq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gyzluygvz.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gpxtnfbee.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/ggxlplzof.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/glqtecbuo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gwqmmnivk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gmtcxdwjl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goqnmovfs.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gzoxxdxhp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzrnvrkpo.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gzfeglugg.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gextdzfcz.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/guortutqr.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggphkdpvt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gqtqgekwu.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gizqktdbb.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gieavcxcf.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gtrfiquqn.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/glfjicsyq.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gjavfoaed.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gaciatyqc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/glwxhqmvn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gakvlzdtb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gezrjkwhq.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ggehtemgx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gvqrjmktm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/glmqpwvwk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/guxlzyenn.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gfzmdmexg.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/goqjtizvp.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gjbwkoqts.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gphptktke.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gozvqxnlm.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gdwhzcpfd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/guzkgwcbd.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gvtidhmvg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/godhvjryc.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gifnaxibs.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gpfwcuvep.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gdwptbejj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/goisolkin.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gxfzuyfuo.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gubocixop.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gkdzxpmaa.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gdlnyigkf.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/glmtzfocv.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gfrnmopeh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/ghualbdgc.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ggwveriis.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gtjlsklgb.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcnbzjnge.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxuzbbjwk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gktrdiauz.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gecpmssev.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gpbvmwutu.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gltgqdxaa.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gltgvbgtu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gzafsasos.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gridpydcq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ggkbdwwqy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gcthjpvvc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/glppdjtcv.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gafbxchqm.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gmspsmibu.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gjmpdcync.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/glqonaklq.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gvfniierd.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gkefvyrzj.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gnkwuhgcp.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gaprkczko.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gtfutkmqt.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gqixvolmo.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gwzhgpqbs.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gmrzdhuou.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gkctushga.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gnfavzlbv.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gevfbufrt.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/glbwyzsnx.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gsvhfqccc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gpumsdkot.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gntsacfdd.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/ghlrtfxwa.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gifvsgrfe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gbbtsdrdr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gjgjvbjnf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gylsdzkcq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/glpfpfaij.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/grwbodgzu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gvwflxmlt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gndvnbcct.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/glcefwgji.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gjydnbrbw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gdpnytibd.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gofxpaeta.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gliciouig.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gelgduslc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gitqeuucz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gfnkrfaly.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gmxoeewmv.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gecxssass.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/ggodylvni.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gxlausgcr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gzmgtxldt.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gvnapehqi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gmibyacnb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqausiluz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gwwkcjngn.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gonaewiga.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gpodquhqk.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gebqvefwq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gshnwdaos.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gbouiovbf.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gzeqjwdzr.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gtctlrlhx.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gukofirga.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gwnhnsypu.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gdfivaqyx.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gdlpcrrdt.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gjkpcumse.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gfgyufnbq.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gkahepfkg.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gsnojfdwv.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/goitgiwae.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gfykphadr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/grhlyaxfn.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gunpjcgip.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/ggubmzxuc.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gxqpepnff.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gleqhxaep.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gpycdanwo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gmqoxkdvc.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/grmmctoqh.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmwqsfgyj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gbxbpnphp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gahybnquw.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/grodhpoyy.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gnuqmsayw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gxbdtwicr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gkbdlwfwm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gkpfrmplq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gxihyzpfb.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gzsuhreqj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gqctvlkle.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/ghfvlirlj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gtbsweaxb.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gzbbahxnx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gosjfewyq.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gvxytibcj.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gglvpfhzh.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gfuvkcypg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gataaaqqb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/geedveyiv.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gawbkkufg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gkmcbghbu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gprktsubl.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/giplbbepm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkqyryuzh.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gbzjdwseb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gedropqeo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gkrzkbohv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gnyvtojqk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/ghnromthb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gzpvqwfzb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/ghcmgylwc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/grytjqjfh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/ggzxrurgf.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gzxannoqf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/glkesqjjs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzlkguvbi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gtqanpxej.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gmwjajwxu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gtumjvqkq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gchuycxcj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gnknmukwl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gwqtrzdnx.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gmllpatvs.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/goqjsqwmb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ghznzqgig.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gcwxiucvm.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gmomzpgjr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/giokfyvub.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/guebfvnzx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gvqlryvty.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/grbgchuuc.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gvoffzwea.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gqvngnxxl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gdsrbfbtf.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gxcnaspwa.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gecoluhyl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gyphyiyci.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gfvtvkabn.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gbphireqx.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gzldpvnnp.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gwgyognhh.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gnxtmsjju.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/glfxmvprx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gvglnsefi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gbznhhupk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqyivozba.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gdpgirezj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gytnvigqt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gflmrozfi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gxwlpogqz.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gtzioacjm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gtdjnhhtv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gekxlxkbl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gbvcoixqp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gcylurvht.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/guxmmqfpd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gypnuwjsw.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gwzzascmy.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gatdierrf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gwqbndzdp.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gzwuwviex.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gzkkwgrwk.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/giqvdyaae.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gvvvlcaxq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gasshcjkf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gjsfbqhxy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gyjzmbdco.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gdamkyvbl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/ggvxksqxq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/glmebuwvm.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/giwcsnyiz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gyyspnaev.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gqmtuamyq.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gomihpzmc.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gyayrzncp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gbaxkzsmz.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gzvtinnyx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/grxozkiku.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gfysjfbje.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/glzzxslef.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gnxrcnijt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/grchplqji.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gidlrlelu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjuyifpd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gwyvpzpwm.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gulxcnvmw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gbsgbyocr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gwljtjier.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gniazaunv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gatxfxcdr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gthjqkhpz.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gqtqbzsai.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/ggbogrbwy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gphcbsbzr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqstkotkz.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gdpgzxudr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpvbzwdlp.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gctsrpksf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gppcwhzjf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/grkknpumu.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/ghgblygfe.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gozeydbju.sHtML


<!-- 参考信息 -->