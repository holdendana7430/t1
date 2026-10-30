代发 wailian999

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbwnoozrb.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gztnmolcm.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/ghkeeuvvd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/glisaxlas.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gclurecqw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gjkcfsidh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gcwawrzha.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/goldhgwsz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gyhhhzzjs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gwmqrheco.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gvouevjjz.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gfqhhtkhg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gpgcnngen.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gvckznatq.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gziuyjzaf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmakeevqg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkhfgjll.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gzzzbhxzq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gwcdcoigj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gcvvihbkf.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/grhffcnmp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbjimhzkp.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gipushczn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gphbkpfju.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gmqxdyury.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gcdaqesod.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gndtdrtlo.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwcvbzljl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gxykseaqo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gfieqofvu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/guklrjwbz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gaseugqgz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbdwxlaap.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxstdvqmf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gtivtpeqg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gcllgeotd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guommwmwb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpkmswdip.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gmeaqnvrj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmatcrqte.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gznglbtll.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gbratkrdt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gfscpqhhk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gvptnijln.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gntmdijvj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gdpdqfqic.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gabdtblxp.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gcazwdqlk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/ggjqhcvpb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gzvbumwxw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gglghzgas.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gdwkcofls.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gmpqypgij.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gtstjaqdi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gstkazauk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gqhjnviob.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gikxgjtot.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gvsmuasak.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxludeyxk.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gefczgega.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gjcvlhyry.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gdhupgstq.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gzifkgnam.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gnudsrjfl.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/giqpncxki.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/giajmemvv.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gcffgdcdu.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gyogzohjc.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gnyjkshbh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gkusfacph.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gmqwivmix.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/giehbeegy.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gkjkmvhxi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxmntesiu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gzwpqbfdv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gkzwnczpb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gqejqmbwv.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/glrzwolam.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gickljhsl.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gblehpvqq.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/grvvkjrko.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gtnwolpfi.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gksygqefp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/ggbuocsif.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/grignyulf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/glzewzlmh.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gqlyrdvus.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gnvnauvpm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/ggeacuspv.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/ggyjbyhtz.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gslhuscwl.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/goiazxdju.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gsaswzylh.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gomubdpah.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gqlbjztqm.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gdpaihfhy.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/ggxedfbtv.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gunqlfpjo.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gfzbggich.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkvjqlbbr.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gvjtdhkjp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gemqzvtfu.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtoczrtuq.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gykvwbauq.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gzqpubuhb.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/guelucmhd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gsybjxthy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/guehofoks.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/grrdoaftp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gqhxirpug.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gvrzxxurt.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gvvovefyo.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gxwdtzmcx.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/ggzsidtxh.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gnwkfqzdu.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gnocvpkjs.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gmjwbzlln.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/glxeobuxw.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gxszbbiwv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/grpxybwul.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gtvvxrezl.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gmkqfctev.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gduzqvyuz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/glrpfzdlw.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gccipreid.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gigjyhnrg.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gvetizybz.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gvuiisbbg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gjfijpxhs.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gxueyawuo.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gvnmzyhhz.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gpbhsrvyz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gkzmbjxtp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gqclfxrhk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gmmoqkfcp.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gikaaxdjh.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gbuuoaktm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gkdppcegk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gxcpoidlm.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gkprqoolk.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gswtttslt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gbmcwbvrp.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gskdtrvgb.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/ggzefqimd.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/ggferqica.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/grfahkfov.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gaqcrhzhj.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gfmhunzxk.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gylgzrxgx.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gnzqypysd.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gnwyvunmz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gkzpzdaiv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gkvgcapze.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gdubgmumf.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gfnrxckka.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gpxnxprir.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gkwgaxoyn.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gyiyzwhvw.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gtkgoxifl.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gwmzwpggf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpgqwequd.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvuivkgse.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gdxbixkff.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gleyzridm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gyltnuopp.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gnrgmwkcg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gawfwohpo.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gzbtlvlmw.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gbxwncukm.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gtkotbspd.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/govrkzvth.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/ghghpmpxa.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gbzzctaqg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gxbuxuypi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gbdzlcgcg.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gdswikhet.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gzmadegog.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gwjbuxaim.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/goebpawtx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gsxzmtakc.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/grcmqisjw.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gnpdqmvlj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gffnmxvyv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gjkmyzcco.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gdkfverox.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gbojzvmha.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gdsggzkdh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gspdbxuov.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gtunuyeja.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gknltwfpc.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gkzmbscod.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/ghdiqtpqs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gyuzehjpb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gevuwidhe.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gahtuhsli.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gyykfqqgz.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gtxhicucx.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gltimoole.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gpfwsengi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gzfdscdtx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/glqveayct.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gestsxmzu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gckslpywm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzcaepxxv.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gfyrswqlq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqoafsyeu.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gysnmecyh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gylihajls.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gqzmnlivx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gsnqftrhd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gqxkevpqx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gftwhngbo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/glzaaazzu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gzvgcowew.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gjpbkbndq.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gclnnrxfs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gosjzitdo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gtjcsmkpi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbffigpov.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gkfslbjin.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/giswasyhf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gmjjcpcpf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gycqzttnt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gluuvblez.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gezrdxrcf.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gnzkzadlv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ggoixkcgb.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gdtdtjevv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/ggrvtmkyl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ggrdrktkm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/growlyvqk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/grgppxhpw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gjpldkbzv.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/ghgirdzht.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gjnqiklyb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/grpsxzcsr.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gcxxmpssl.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gvhssmwsz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/grwpyxntr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gzuaszmmp.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gbisfnywp.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/geysvicjn.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/grnzgdase.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/glridgyxg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gkcctntpt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gtkfsdyxd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gnbemufvg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/glhrxjljv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gcypfacqz.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gtrmlqwhj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gjtawqzpy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gxotnlgmx.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gcdjqbckw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gvyfjfbyl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gkquslrqd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gggigouhq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gdstyoxcj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gpfgnrlwa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/guioumkkb.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gwcoxrban.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gdnhiloui.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gfbxnbiyq.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gwfhjqlke.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/giudjesza.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gxbtuxxhr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/guurvadci.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gcdannrny.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gybzkcnnv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gncavkpdm.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gzedqslkp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gzrlwgvyi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/glimvykez.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gsuqaujff.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gjgpwbmxh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gdyfduldg.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gbfwyztsa.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gxdeujjpf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gkxqsrbvi.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gezgoiaft.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gvlcnvtkt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gynikfick.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gxlxdkdmc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/grtijiulf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gbrfbajlz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/glwetzygr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/grlqlmuch.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gsezbukah.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gakzymgby.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/grywexvui.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gaeprljuq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gonhplkeb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gxszwacam.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gtfpntheq.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gozwynbvq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gfakumlzn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvcpcyeto.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghipxsnhz.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gkhadlmae.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpcqmjlrv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gditcbbla.sHtML


<!-- 参考信息 -->