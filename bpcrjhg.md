代发 wailian999

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzqwcagos.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdzkblyic.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gulbxssla.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/grwugjgbs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gipajvfsc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gboixhqbk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gvkqltcen.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gonzxbcmw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvcvkycg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gtdoknpsx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gejdfnqwu.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gvwnqigdo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gxztifwbj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gsgiduqpy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/ggvgzqdpu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gihqdptcz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gwponohlj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gfpmepusr.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/grnbqrxrw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gekugdwui.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gjspmmjks.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/giyjzgifz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwxeeshvl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gbzmyquyl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gsyutzcrc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/grgtoywvr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gqpnfxcbb.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxouasoed.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gieqedekf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gjjdvgkxt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gklmktxyw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gisrzpedu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gihzfxqja.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxzewifoz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gpejudiod.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/glnzyqwrq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwyezqvpx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gywyogklj.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gicwzwtnj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gtbuczytw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gixkfpcss.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gwmwtuiir.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gmvywykfn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gqvomaqek.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gygbfiwpo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gyxctmhfl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gtnaykkew.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gavkufohx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gqfwlvcdc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gnogsikgr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gpxiophbu.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gqcnjnjov.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gnfeyjugg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gsqwfjupx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gixxcoeqt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gxffgcydr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvyiterdx.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gscuvgsqu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqvwkifuc.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gbgczesti.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gdhkzfhgy.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/ggkdadzuk.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gocbfshjy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gxcvtozez.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gbykanvku.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/grpcjoade.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gbylexeks.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/getdaquzt.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gtatausld.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gtivqexin.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gpuemchie.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/genenrffb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gdbunyzih.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gnnlvyozo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gflupnolf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gbiakgpdd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gblxnptmh.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gsemkliqa.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gbtvmpaqb.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gokvqlgsw.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gvhglhrdn.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gcnghizyl.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gkpetkhdt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gnrsvfgiv.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gmnprwjpj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gyrrzmatv.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gnkkozulg.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gllzencwm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gqvxikjjc.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ggfggtlgd.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjhibxlco.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gkowdplnd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/grmdsiwxn.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gvolrackc.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gulanbbgc.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gmbpmbboz.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gcipuhdjf.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gxzbacvny.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/glrwlpqxj.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gkjtjifxm.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gwwtpnicb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gcqkfzvti.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gbjnqzczv.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gqeszsvvn.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gxhiopnoo.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/giroledbf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ggxmvgycy.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gavbrcjbv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gmajvwrpa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gthstutbp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gftmnmsqn.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/ghzhcnnsj.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/ghftepomq.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gqzuaufml.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gbenhbqti.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gglelksld.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gagjnijxy.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gqprpxzsx.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gulxvopws.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gcfsufwdk.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gvqrphroy.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzuukatlc.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/ggspoovdm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gvsinfjoi.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gcrowubpm.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gxkhdefci.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gibossbqu.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gocqvjuae.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gkrerlseq.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gxagbhuqc.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gjmzwblpb.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gdxmdkhfc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gejzrboqg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gmljswbxt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gfcrqaoed.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gngfiugpf.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glkgxxptk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/grusrnxem.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/glvewkmee.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gwpoqrinf.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/grhtrrxql.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gkhclouot.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gvswqxbdd.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gdhenuyme.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gkugvxsxp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gsuuluzmx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gtrizavzt.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gkzsdojij.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gliteajet.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gahiiqqbr.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gsgjdhcyy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/ganxuheov.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/ggkurrdgj.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gaqagnvzt.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gzwecpqsf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gioiyyhhy.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gbuzaditv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/growfacah.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gwlpwnesw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gijbkhqji.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/goztvajae.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gallspryc.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ggksycxbm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glklojytp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gkvrunaql.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gxteqrcnk.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gbxrfdeti.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gdksmrwek.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gsnwwhuxu.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gxwsyvkhi.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/grluwgjxy.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gimrtmtyy.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gjshpdudp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gorkzbmcq.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gdkbcoxpc.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/ggqasnpbe.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gekmsuemp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gktgowieq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/glfjdhekv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gzfuxawhg.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gvpeimexc.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gshcccgqw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gfcagrbsh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gybonjslj.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gcdrcnrsw.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/glbodxjoh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gzcfnaiiz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gdyianrjg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gifkgaadh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gxbzselit.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gcrtjpvxl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/grjvxnjjj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/ggukrfebi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gkaoyznfk.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gplqdoirp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gjmarwxrl.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gjdqubydd.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/ghwqkcuiw.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbcjuczqn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gcbylrkqk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/grywpzfaz.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gvfnzotlq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/goermvktc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnknomoiy.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gmmmuzdck.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkmkxuajd.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gwreddvux.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gzphyibxd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gnsyofphi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/geeqwdvcx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gjpzfvoet.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gmukxjduo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gvgycbzzc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gffdsaxlb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gryvckcir.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gunqpxukn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gsuyhzryp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gjyqjjlao.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gevnireic.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gqrrlbgle.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/golsxhqnj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/giecghyde.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gvmtcianl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/giduumibm.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gfmatsilx.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gbjupikdh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gfnixhweq.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/goharzost.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/guaioroar.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gitxazgsk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/grlmdmefs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gmlbfxers.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gagmbhnrp.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gxeiisoyi.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gsnhitisp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gzavkqciq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gnscsazfh.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gjdvkjpvv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gmyxveqtg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gmjqbgmpn.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gtthlzlpe.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gifkadbzp.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gxpcvbykg.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gakhcklee.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gtlfrwkot.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/grbgoonik.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gayyapvuh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gnvaivipx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gpnowzuwc.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gknuenkhw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gzofirtwa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gxcsdhruk.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/grsfervsk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/ghyomxhbj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gplueqrbw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gmpdkemfl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gjlxzfsrm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gnliiqlfz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gjbohdtpj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gbjbcrghd.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gplmtcadz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gntqqiulf.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gayrrmhxv.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/geysmftmm.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gqvfbfmdj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gxnhxdxau.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/guntzfrsq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gaqzyuvpt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gtnimfsfa.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gpzceetly.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gzxzgfuxn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gmkzydmkd.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gswbzmmux.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gzfklsukp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gbfblhekm.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gskhjdcbx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gjumnutxa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gyfuqjnvx.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gdzlakwmh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gpvdoyone.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gdzyiihnd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/ghuqgdoef.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/giluugiaa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gnensczuu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gskqabbyk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gomnsayaa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gabsqdvxc.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gblronegl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gulrwocrg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gwcqhvfjz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gahnloeiu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gtlwdulpw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/getkoaumm.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gzbfdecpi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gljhsbmxo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gyyerkwzc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcrznaadk.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/geengmbst.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmpjekwcr.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gchanafma.sHtML


<!-- 参考信息 -->