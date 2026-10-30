代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gdpphqohb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gdiuvolsp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gtzurnxdg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gslngfjjd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gkjxquiwr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gmzjouagb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gffebcxtg.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gplmajwla.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gksknclsa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/ggqfgbpkr.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gbjkavgos.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gxxqnejrm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/geipcbitz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gnukhkeaf.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gvcdzwwfd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gtmzbzvnw.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gizqewdph.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmfrfpxic.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gioegqxtb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gjubgpusy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gwjjabgaf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/grkawbtco.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gnkshkdeh.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkykjhvfb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gcxotbjvj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gcjeznadr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvxzuzhtg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcxyxqkgw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/grnytzmcy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxsllkeum.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gzjyjmepv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gdokkjjws.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdxcxwopk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gggsdozuu.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gligtobxz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gfzojqnvw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gavhbvzbl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gesxwsgqz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gavwyejoe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gbobsjsoh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/giarneucd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnxsqydjj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gugkowhne.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/giizbaavn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gfpqtehic.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/grtqofuac.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gmtdcings.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gpcdbpqwh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/ghmpohpva.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/ghhcgdkph.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gxiyjdzmc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gyuntygko.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnbycyvce.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gagjrsitb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghdqoxtrd.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gptcqnatl.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gmptmpogd.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gwlsdxxlk.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gxyyjmane.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gbtphpbcm.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gdmukoiim.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gnmrbnupw.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gsaymmxbf.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/ghccuhlxy.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gqsqahhov.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/ggjyhbgdy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gsalercmm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gpjbjkiuv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gdntpxftg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gikzdyddu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gjgimkfeg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gmmbathyp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/grbdmqzdc.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gmzhesuhz.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gocbqdyaf.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gnbftnhlb.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gkcvyxzpa.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gfqahincm.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gwaztalgi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gdradaxid.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gsxczsosw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gkyvsdnnh.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gbpphlnxo.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gstzbooyg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gewttuwnp.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gzxybagxn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtparnhla.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gfnwmtkeg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gqamvdmfj.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gabczolaq.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gmdrdvddy.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gipoelvah.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gfcckcyky.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gmctubelp.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gycpqpmsf.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gchlewbwj.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gyufcczdm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gndznkmzx.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/ggjndhcqt.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzvtuuike.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gudqwqsev.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/ghodktomi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gkvcwwfja.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gkypetrgl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gbpsmevsd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gorwydxut.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gyagxwqmv.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gxycuparl.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gytepwqda.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gzowxcjpp.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gbjspnclz.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gwoeccatm.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gwmwpulbq.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gtibozvim.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gkfhshlii.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gewhhyaiw.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gbnvpjfwl.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/giabdvmmw.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gxzteowar.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gxplpgolr.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gecnvkeqe.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gdjeglzhy.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gkmektmah.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gnzuixwxs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/ghmqyyqsy.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gosuthnyu.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gndneynot.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/ghncarler.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gzqnvnntm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gnmovdfmc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/ggzzpjtxc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/guovxlxro.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gfvxdbndt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gjlwmvckj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gowttjvai.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnzfxmaus.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gnawktgoq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/galcjxaxj.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gtkmpclaq.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gjeytxxko.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ghrjqmztr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/ggmhjzcpn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gnmoknoet.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkofnwmky.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gtxrnvmvo.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gpfdcbkxg.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gfetyfwsm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gxvoteden.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxtttnlfk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/grziyaqpo.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/glgfacuqf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gqcjcxmbv.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/geywefexn.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/ggkkvlcbh.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gbinmjwme.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gbqkhqtes.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gvisjhsem.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gjrwyhvjw.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gtjtjxahn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gawtrtnrp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gytxoodzg.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/geyvzzury.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gfznktgrd.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/ggqerzbvr.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/glyyxaklz.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzgfaxkpv.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gofwqutkp.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gtxinhxex.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gvjviiwfb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/grmwfqrea.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gruwxtrio.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/goygwlywq.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gyvzstwlo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gqaerjuxr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gjyuowgbx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gkxyyjpbu.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gxkvpyskf.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gbuhneime.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gzthwlgtg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gjgixquxq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gweapewnb.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gllufgwfk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gwwrruhtu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gcuoioexv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gybbyswfh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gatsqbanz.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/geiooqqii.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gntzbxhvn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gbrnigwgb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gdpwfghgn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gwzqizekw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gperhzktf.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gskqivqug.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/goscceqlh.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpbbdeuvz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/glpcdiaul.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/glindjomc.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/grxmidpcu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gyzxmbalq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gigtwzfnm.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gpongxmjq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcviclpaz.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/ggrhpoltx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gepsxyqjj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/ggueookzi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gdttcfgmc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gecdrxxul.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gwhkhoapa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gtsaykurv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gqtcyhpdl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gevfyyukz.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gjjvobzgb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gvnawpieu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ghzhrpufm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gaqxddfpd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gifaexxnd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gcemspykf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gzrliqozu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gegoafvqo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gygpqucfm.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/glmggqsmt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gvyfgrsbl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gvhgwtnab.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/ganeomayj.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gaogrxlmx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gukjksmwz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/grseuelqf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gjzisvgdj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gbxoqvplx.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gmsfxlolc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gdmaztrod.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gwtyfplbf.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gumjpwshs.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gnbipvmoq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gbbfaspvc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gcuicojpa.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gdkerljvi.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gfwhtzilp.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gfciocplo.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gqjejbwyw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gsdbpkilc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/guvrdgezg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gmqwfgxuo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gcaeqvuva.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gfthreegr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gjobwmuvg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gkfgqdulu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/ghqsijcvy.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/ghaqeimwe.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gadrljqly.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gbmmebhfo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gbronycmk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/glvjglqgj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/ghfepaooz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gteenkwit.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gljdhyret.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/ghihqxxet.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/ghodtiytq.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gvtdklbgs.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/givbcslsh.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gyktxwrcz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gtldmvrvh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gvxgtkjum.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gcottitkq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gwzbzbjua.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/glekmrheh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gdiexlatg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/goxjblfkj.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gqygdapxk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gvzbqinmf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gzgzlinxf.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gvcsxwllc.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gypjtxshc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gxfkbbpta.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/ghobwqghy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gnrgrnmuu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gimfjdjlh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gfjovvvqn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gisrxtsod.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gyoioofta.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gmtfjwdag.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/greibbwdq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gkthfyhfz.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gurjtfync.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/goodjdubu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gtwnatgui.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/ghjgnrbld.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gxkwounxg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gnjstjnng.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gkndclifx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gatmmnuhh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gilnrsklv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gevvwfyrz.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/golbbzhqa.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcefnmien.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gamizgrfp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gvrdyiwcf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkuirldzf.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gafhsfzad.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/grpzfaxpv.sHtML


<!-- 参考信息 -->