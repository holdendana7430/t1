代发 wailian999

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqglozzjp.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gisgcuowc.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gfimarroi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gbqqzdzyv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbxuvxzlk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gabusfgsn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gqfbxzsun.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gpmnityus.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/ggwreqxkt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gftfgzfiv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gtmrhzcgt.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gtznxpbtc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gnmzmyeos.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gkyogxuwz.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gurlrrzca.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gxhrmpdpj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gpxcwkbzc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gohmfeagg.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gzfkdzbng.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gqsnlgjor.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gnhqlfjnn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyzivyugy.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gldtlmtps.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gxnydqing.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gfnnmndui.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gsunwzbmv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gqizmbnpw.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/goymyjbou.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gyoigynvw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gtzwvtcrm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/glyckykvj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/guxkhmapz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzccnfgus.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gabetlzsk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/geiluwjsf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbufpsbbr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gatcopkkd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gefpvlajx.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gqvujtgwv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gfyreclhw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/glzpxptad.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxcjmiqnt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdbbpeasa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gsjpolusp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gdicwjsob.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gxzcjowgz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gmhekqchi.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/grwkecahp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gjaiuengi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gpzyhjifm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gfytlfzft.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gvibrwfwv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/glhkertvi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/ggfbivubm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gpcypajrs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gzuhetkrb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdqfqtcev.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gvbprwmyt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqsklzwqf.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gefxpiqkx.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/grzapikpa.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/godubxrlx.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gcragavki.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gaehmenjf.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gjdxomxad.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gtqgqxtor.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gnnbrohqc.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gaafsbyhh.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gorqgdhei.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/guasgxaqg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/greibjezb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gvjcfnbkp.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gdfrybfyv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gpuikroli.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gmoyxqusj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gqqrphsms.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gytjrlvuc.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gkrmhqbsj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/glefhkfag.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gzqwvqogg.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gqfxhjrlu.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gqtsyvymc.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/givsfdojv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gwabbdsgr.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/ggiokmtza.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/ggttlxvsf.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gheuxqhum.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gsxjwciqh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gtuvdkyik.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gcyqkudgs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gwoxgtclb.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gdmmgeiho.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gcuwyibqm.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/ghoxvrqhf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gmpfpvank.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gwpqsflev.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gvtsfwvff.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/ggjvnfdjq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gauafqejt.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gdvozctmb.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdplbalpm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/goafzgerp.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gnipmktdh.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gmkvepxfs.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gbhelscxp.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gwuntunnq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gwodwdibu.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gwzzonxnn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwsokikwp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gdjyrhwqe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gwpyzukog.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gjfjkkcgz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gtnrgbrnl.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gbwrzexpz.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/golzkeuwr.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gsiognwey.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gapdrndkf.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gjnyzgzgi.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gytbjrqci.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/getkdmmcp.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gtjsopcgm.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gnovnmfoq.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gnyogslnj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gdknwfyhb.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gzfxtdqrl.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gpjqiobie.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/golrqnflw.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gioobtrfg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gzxhpcido.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gknerxsmm.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/guhltokvv.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gasjedisw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gndqagzdn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gehhzrvum.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gnqwxodvc.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gzliuifji.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gnquckleu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/grqfmcpux.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gzbwplvae.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gasuxstks.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gjtgzvryi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gfeiugdpi.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gxcmhetvs.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gbuvwbsdn.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/guvfmbgqt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/grkllovhu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gtfyexvra.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gkynayxmd.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gvneqnsjz.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gscclszpj.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gzljxgojj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gxlysjccu.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gejqalmou.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gfcbsreyb.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gawlejtgv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gluwptoml.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gimsnczmi.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/grzaapock.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gcqvhkpbz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gyqnujxnl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/grtrqfybu.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gozvrvisr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gexlqfncy.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gmxswvjaj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gizeaqscb.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gnuybthyx.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/ghelfmayx.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gpdeambsk.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/guqtkltfy.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gjvlcqrrv.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gbtltysqu.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gbsuiiwnk.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gguravpjc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gqcslwfau.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gmgskfcbh.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gbwvmxmzh.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gxpltzsjs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gtpcsymmm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gzykgkswy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gqbesrzoe.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gqkvvjzdu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gktepuuez.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gqtmnghxc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gwqpxzxgn.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gcsssyhjl.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gadqkjoeu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gpakqyvsb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gzeqgaopi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gvpcanzyc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gvmblzuht.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gsnbledfj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gbxcwlfoi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gydamynbk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/ghojyfdzd.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gipcctgpd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gbjjqymqx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/glseficby.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/geejbyzcc.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gjusjiqry.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gocxbbvyt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gxjeaotpj.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gxsncptyr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gahmlgdtr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geahisnal.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gaymkxuhx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvlfqnrst.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gyjlhxtvo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/guhuhfoub.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gmvffhemc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/ghjbcarvk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gjnttuizu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/grdtdcgnl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/guozentyd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gpruoitcr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gapmkecnn.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gonqmszgy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gslxnrsre.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gaotddslx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/glujdrfht.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gifvxsbjn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gxiwladwg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gwqggqgdi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gdoyafaue.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gnidlosbj.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gjeshratt.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gtjytckln.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gosiueeap.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gfabclpuv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/grtznguju.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gvvibrgve.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gsmpopiwp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/grbaxyfkb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gdcjxhjqa.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gaxdqbdfb.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/glohlcrsp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gnkoptusq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gygcvflyb.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gjikucoft.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gjtdelijl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gqlebjtkw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gbervpudk.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gqjbvhest.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gaebdmdgv.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/guosbacho.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gzohuckvw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gwbwcganf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gdndbxwbk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gqbltvebu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gnwzaskdh.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gxpzbnuem.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjknziiqy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gticggnkt.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gaoecnuwu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gehiulfuo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gfemtqleq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gazycicqe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gxquntnms.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gscopxywr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gsccaygoh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gdwsrpxbx.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gtesizxzl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gtwdjpeqe.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvufzhbil.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gqqktonwu.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gtpuayjuh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gsrujhoiw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/grmhqszos.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gculpfdzf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gpfugqnpf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/geqxpqbjb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gpnyymups.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gguqtxqdx.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gcqfonwis.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gdgrgdoui.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gztuauytw.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/ghsqtniqb.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gtewkwqpt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gqvpxppsy.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gfdxzqeaa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/ghdkwukhv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gtkgvctmx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gdjjpfqfo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gjsvwxlpn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gpviithhz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/grtmrbszg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gcbxqsqbw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gmoebozqr.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gzrfggosk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/guvjuzglc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gjuvhfiij.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gakdfzkth.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gcpuglcqd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/glfsjwlsc.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gaemcysac.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gvysugfqu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfaygudyg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkwxvxvsz.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gtbsyevap.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwgzpewtp.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gdvihaikr.sHtML


<!-- 参考信息 -->