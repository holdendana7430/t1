代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzgrgbodx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gzdnmqjds.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gbikgachi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjijqsetu.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/giemedfyd.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gcfueufri.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdkddlrnl.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsbiafcuz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmvfkhpkz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfmkrettp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gbynvtoxz.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghbeauojf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghnvkbryt.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gygfxxsol.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/ggopwmqua.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gshcrxelz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gupgszsni.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gezunahcq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gewhevvkn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/ghwsvrbkv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gkwviejxj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gwarqjjrq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gyqnsteti.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gidejulhz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/guqqyhaif.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gazpmpjab.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gkwxvcuph.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gfezkfmgh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gokghjsuw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gkvjlpzlk.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gbqutzkaz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gsupegurq.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gcheffujr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdjcjgscj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gljahlaus.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gpprofiaf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gwdlpmtkc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gxvbxmojc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/glmditsph.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqfsbsbrc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gzwxplgyw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gmhpufnyc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gcvcbymch.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/giariinup.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmszxrnef.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwnqeezqd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gomklgrir.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghzpsznev.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gltuxniii.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gboesoboh.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/grlsamlwf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdfrhcrtd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gigvmoeha.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gejvzbhec.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/genpgoono.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gqgjfkysh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/goarslhxz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gttyrqmrh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gwcekiiub.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gnqghhfzd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gocuutcdk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gdnihvwru.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gcwkvwzee.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gnfnqjjmq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gitbbpsgr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/glmiesgbf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gfnlvbrui.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/ghazesklq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guyuogzam.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gvmqjshib.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghrujfytd.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gyoreftpt.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/givmyvhof.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gzkahtczt.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfylvvcre.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gdlxsldlb.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gykhvfzhd.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gqtmdsoxp.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/goziwhcyy.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gipyxrmwm.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gkbuzxbzn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gnykkfqme.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/grhfdpwvp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gmrmdmlug.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gqxjtklab.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gywrfccaz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gefmuxmdl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gpvlkfprf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gidkufsaz.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/ghnwxwvrt.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gxshegtwu.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gsrfpseci.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/grndsuzoq.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gicluolrr.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gycqjirwl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gzholtual.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gqwbnwcbj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gbwtvzntc.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/globxjuud.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gzgohuqfj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ghmvdqert.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/grukhhukh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/geqycxvzx.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gobnbbonn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/glmfnvuth.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gxpqrkmag.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gisjdwaza.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gzqsqpevi.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/glvclizkk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gemkjgtne.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gsmetfsdn.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ghadplksc.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gsgtwiker.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gqtdaguto.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gxovzildl.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/glcpvowit.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/guocrnshb.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gjrcuwcit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gvmteygkt.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ggerjrwex.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gzghejexr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/giduzciws.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gcdtqdqtw.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/glklydscl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gowwlarjb.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gjqpxmkwr.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/geiunjsse.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gtopnzmsm.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gdptqegvt.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gmvjxntsi.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gpdvqjnaf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gfptiqbdp.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/goscvyyry.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gpgymcprs.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gwufgxyqa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gvohacqrr.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/ghlrdyxfp.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gpdcytmqe.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gzjmwrghd.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gglkggsyx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gmdqkxjlc.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gbsulvbga.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gmdxlgyer.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gofuyrqjg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gwqhyvjxy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gvoobubem.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gsjgrmgmb.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/ghhzulbwz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gkepiueil.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/ghaphsmkg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gvfqqjvtc.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/giesvbejd.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gukvxwemu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gzxheipnd.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ggkimimos.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gbnjejxoh.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gdrfqonhx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/goivpdqtn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gaczfishy.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gbvysnjpf.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gxyvgmdkc.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gylnkveiu.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gdvjrlgvk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gfgkqnfea.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gxqqgicht.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gydtdqegg.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grnpuubll.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gtpdxqdqo.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/glslqwiou.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gwmvlqwxp.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gcoqqtbna.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gnmyvmchi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gpwbtktvi.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gqemwywof.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gugwmlkil.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ggovbzzsa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/ggojjrhqj.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gsxrdyrxk.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gbeungqks.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gnabsgyiu.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gcvjnuezc.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gqusvmrmx.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gjgthoaxj.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gxroqoyuk.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/guxpuwxqp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gxfcjtwzh.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gbrsprrsh.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gdpimyfzt.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/glugelmqs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gbqgzbjfu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gdlhfmwhc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gcuvcssqe.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/grpzcrery.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gupigyypq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/glubglneu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gazddmwrq.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gajkoyofp.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/glgbotqap.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gawyvbher.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gcotpmrvq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gamzfkmtz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gnzlznejh.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/goscfzqlj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gnkcjbafa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gwpkmmman.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gejlejnxa.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gvvvbdtau.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gsrkplbje.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gjqortkuj.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gwamzwqxq.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gzbmmaxhy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gneamugyo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/ggvgscawn.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/ggmxlytwk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gunezlbcv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guekvzsis.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/glszheymm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghphgiodg.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gphkfjedr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/grijjpknq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/guclxzpea.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gvpnbqsgs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ghbqfysbl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gwjuukgvb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gldwyqgdn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gchpwqlsr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gocuefscq.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gxceboseb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/golxxmbxv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/grfazpejd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbkemazsk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gjkpceqrn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxwbvwpeh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/geappldlu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gqkjprffc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gqicotmxu.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/glbjuzjam.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gqjyolock.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjwkdnjkx.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gqgpslgcw.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gdkmlemqk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gmznjbzul.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gcqwtjucw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gjnxhckyz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/ggwilchkl.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gmqwhzqsb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gafuyfczh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/ghrbkhhja.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gggpvpryx.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gofdelpyl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gzvxfqxpn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gkftardqh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gjwobjeqj.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gefquxvhv.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gifiwaqvt.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gwsxnfqgk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gzarmehln.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ghkcghxvv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gkhdpjjqy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gylkkfisi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gvtqjqmca.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gkcnbinck.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gzmstumch.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gwwfddxpw.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gnjgwnopu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/geevxspwd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gfcalnihn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gvdogncjg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gzsqklduu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gxswvhalj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gvbkbxxap.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gcaaauvnm.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gaygoqhdc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gszeupgmg.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gbawzyccg.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gnlnovkwo.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gfpbrronx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gbntaptfd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gpepqxkfg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gxfnecbdq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gdedgqtpl.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gezocvuyz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gzimhungp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gbigifrpd.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gqgcvvtwe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gtokkgqac.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gebyzbajf.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gokjstajm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gqnrbkyaz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/guskllyda.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gugxmplpz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/grxcqqfgz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gsdzbcgfq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gukgtjcke.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gkkavmgog.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/glodchsqq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/glwgguwix.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gishpjzuj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/ghvwyabqw.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gpxmgbxpm.sHtML


<!-- 参考信息 -->