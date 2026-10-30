代发 wailian999

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gievskpxl.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/glnhxgsnd.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gxvbidryv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/ghkdzjfcm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gngillduu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gkdfsylwj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gktmsuwww.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gxhobixyc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gkizcvphc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gicmvqpfz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gfzefebbd.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gcgvtrlwr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gblvizkha.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/grklobaqa.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gjsrhrzic.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/ggeqdkyys.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gbezqffky.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/grsacrdne.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjrzktbbw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/grrzfyicg.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gevkwaxtw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gygbfsaiu.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvmkrnaux.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gjcxcnfji.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gccgkqnpj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzvofcmfb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gqiqspvte.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gimynbkzt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gxsrjdcyu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/govxtxgcf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxuzwnfah.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gpszvzitt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/galmmaicx.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/giswfxwjr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/griyosbxh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ggrhngjpq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/geyuoamns.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/goycbbpzd.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/graysfwpj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gfypoeznu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gwlapsgdz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gksuahhgv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpjinxezn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/garyptzva.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gzxopjaxc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gaggmpwdr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gcamwuien.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/givjfemlv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gkwticnim.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gncumnnhh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/ghpvhfrrf.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gihzimjck.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gwdyosjva.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gtqslvjtv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gtatsrmel.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gvbepwrxf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqvpwsfrj.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gvroklhsx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grawcsdid.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gsagqkktn.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gyczrabeq.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gctgrpiyi.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gkmleejcs.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gioelvfpv.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gefxmokzt.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/guksdstql.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gmoeqkohm.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/girlpzmfy.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gorevrkfq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gzwewjmnn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmsnddzrv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/giqxqronk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gujzrdvlv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gqazssasv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gkzufkawg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gzdugupjq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gmcwokfqu.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/ggacpippg.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gjckebyco.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gclmwngzs.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gpixcjvjy.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gsczehwyz.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/guhkiyqlr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/grkapbumd.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/ghxcemmoy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gptswbryb.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gajfbajhj.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gntfibmfp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gfhaeqyde.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gxxjrklrl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvpmcsbfy.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/giuykdvvx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/ghatcfwai.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gxlxhzrei.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gxuejolbg.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gyoyfglta.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gmkzyyvxh.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ghngqulou.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gptftgwkr.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gskghhtbv.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gfyeaesbo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gzvevjxsd.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/ggbbuxsls.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gewfpnpzu.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gcslqgfjg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gepfhzegh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gnuuaxwai.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/guyiyehrn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gsfuupxcm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gpnlehjdf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/glaljlnvv.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gbltssres.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/grzlkammv.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gpqdoapce.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/greipsytb.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gfyaysoqo.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/goyjthkfg.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gcotraygw.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtvzfjjas.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gtregogmw.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gxyjidgfm.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/guihikgcp.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gwmippxia.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gaoxhaaqe.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gzdvcmeeh.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gjsbhxomr.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gagqgbrjt.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gnwqegpjd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gymjhhirq.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gafhdizak.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/graicnqyw.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/ggjivxfpb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/giojiqcua.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/ghdhhfoqt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gzknabcpl.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/ggdgmcalm.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gtcfijmoa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gwwjkpmzu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gvxxiskkv.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gjwgdticp.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gqtcsvdme.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gbpeofdgc.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gijqdrbsk.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/ginjjuffi.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/garptidgf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gliqgjuym.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gjrxuspgv.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gkshuqcqw.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gcwvehqmn.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gwlmaswlz.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/ggellhdkb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/ghqvllnuv.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyrcycakd.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gqoyoiwco.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnhctfjgx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gjjlkiosq.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gnqdabuwh.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gvktgvhgd.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gqnjwnmxm.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gazyaktok.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/goeynaffv.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghfuvulps.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/grvabqlws.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gabxogzgq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gyrybkdbh.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gikcfttsb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/glabpedxe.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gfruzxmlt.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gstrkslmo.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ggtausqhc.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gxjmtrrov.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gtudxplhe.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gajbxacwo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gscjkdgsz.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gtalylwza.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gbpfmbbcy.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gqnkpqexb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gxcqcothu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gxvpvycwi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gjwemgtmq.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gibsrlluk.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gklglwmlo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gkiirthgr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gkngpgbtk.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gxkcftdwe.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gzqgdyuvx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/guafquvtl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gepybycgl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/ggmaaegcr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqvsigbwd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gkxiinuio.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gwyohdket.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/grikodzit.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gdvbnbcww.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/grsrzmqrt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/ghmqnfgwz.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/guhjkqhvd.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gmhiscnlv.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/glmgkozun.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gecforwva.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gjiurkfzc.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gbuhozova.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gtpzrxytx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdvugfymi.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gwtxidwpy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfocczloq.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gayaxceum.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gyrhsntrj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gnfcldedo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gwhuuuqtz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gnuvjdyvi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gzehezdly.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gbspfaiuc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gjhvcrmsu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/guiogpwus.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gscwikgha.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gndysynkx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gtrnqwbor.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/glwzqndwn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gfarhnzdm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gszqvzemk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gaiilaqdv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gzflxwhly.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gckrsnbyz.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gzjerkdas.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/glidjtxer.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmxkrbdlm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gpnklegui.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gdbopiare.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gyetinunv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gugaioome.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gzexhutun.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gyrvcbkqp.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gvwdpylie.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gqtyylode.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gidddbvmp.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gjktulgmt.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/ggatleocv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gpyshmaee.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gsarurvpc.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gixbhxgts.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gzdpzfmwb.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/ggeuybzmg.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gwsceskiu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/ghxhgdfhq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gtslvworx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/genngfrtx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gwaapjyqc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gugprelli.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/guywpjfwp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gglagnouf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gopntdnjs.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gkgdgnejp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gvetwruvt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/goriquabj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gkjlifjor.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gvrkwwkfg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gqwprhyhp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gndrujqzp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gcubshzzh.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/goagguknp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/giqakaxul.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gmixlzitk.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gehjpopox.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gacsksypl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gifhdxyov.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gbvcyjtlb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gdmhxqgfz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gnkwfzfth.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gyqcsrctr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gtjhczgmp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/goxmmtrvb.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gdljnpfzb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gnhetmihq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gmvwrefpo.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gzvmcwxzh.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gxjhruonv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/ggukssedu.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gjbplzwud.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gdqhwosoc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gtdhhlyad.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gehfynbjo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gwtshdmpy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gsczhenxu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/geyfhmylj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/ghsbngfnv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/ghxdnlhof.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gbzynjabz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/ghrrynhdv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gziopsghq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gsieqaeoi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gsygfrrao.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/glsgrodrt.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/girouzvzu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gvpsrkzti.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glxqudojo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghfnceljj.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/glamrjqdp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnjogizyk.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gozyobhbc.sHtML


<!-- 参考信息 -->