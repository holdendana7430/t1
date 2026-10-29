代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/getcqqptb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gbyheiabj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gmbeferbt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvedvndqz.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gipimskyo.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gjmnfxirb.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpfphugze.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gyaufhegt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjzeeqtde.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gncaywcet.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/glwztcqgv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwliafdto.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gduivkyuo.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkcfhpoqd.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gqciasvwt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gkttqbval.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gvnqitmxp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gmqdyclqy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/glnqxxuut.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gpeadvdys.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/guqnulwhv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/getaqpbji.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gindgrwxs.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gjuyqkaol.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gpbhqviof.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/grmlwsrae.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gwvicgtaq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjbziawwy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/goinovjwt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gyzuxjnmt.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gmhmyaund.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/ghekilnqx.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gqpmeugeg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtjuuxmzf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzuyljntb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gcxyhtsrf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gmldridcn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gkzojkuzu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gudjznlqq.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggydcwdzl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gjswabuvx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/ggdshzcuy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjmdaivyj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gkbcxsokh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggabkojgf.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gepkxlyjg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gvldrfrcw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmbpyrede.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzdgtyrct.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gizpfaefw.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gzyagjxmt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gmcreoerc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gjodojjvk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gsjjfsksi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gyvhwjrkz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gcwudoqol.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gunvoeqcj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzyfuirur.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gdyfpzmpl.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gstgrsyvg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gucdvpsog.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gfjchfska.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gihwtexib.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gwplwnjkg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gqmwfebmn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/grpdmwecu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gorzsichd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gqkatvqyd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpppnbzvw.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gpdoovycd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtktmckff.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/ghuuysvtr.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gagwsrzmg.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gqhoxqtkx.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gwtursxep.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gzmuahkrs.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gaifckvrn.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gxmkjstfl.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gpxlndqah.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/ggcsndqnw.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gntuubvbj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gyyoddosg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gaphqduzh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gwfsjxhih.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfkthuubu.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gnkkmnaoo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gdpwetwxd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/guydloutq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gwxxzfgic.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gcndxsjek.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gnlnnygwb.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gcjzarddd.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/glkhoiuyv.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gvhlcjfbl.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gvmbridgm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gjtignjwx.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gkaizowmb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gucdepsyn.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gwzxuvkpj.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gdhwfxwef.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsitirpuu.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/giiigwkdt.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/glzdmrtwv.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gcepfehed.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/getebqpir.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/grunnezcm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gyecsrswj.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gxxvtwowg.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gayoqdsdk.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gilusbhvg.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxgyxzsaf.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpiwvxtbd.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ggvlyxqsu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/glslsmevi.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gprrefkik.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gxulchxgj.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gxtutvugz.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gkrtcetaj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gbqwjzite.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/guflzxadt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gqhdawkbv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gibjwahqf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gnjrfgapn.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gfrcapzeo.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gjyzcuzdv.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/ghmnvnuxq.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gomihsldy.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/ghnywreuu.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gxylnacmd.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gswabrecl.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gaqtvuaex.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/ghsgjgwou.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/govfkfigu.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gdfffoxoc.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gqaefjvje.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gvmzmmsnw.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/ghgitwhhu.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gaaqgoiki.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gqwkzdjfs.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gnjkzoqvz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gryxsutzm.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gotstgmpz.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gekscujan.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gyvojixas.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gaulexaiv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gjcqbzawt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gkfzjwzrg.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gsrjoefpr.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/ghlxsepon.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gfreusxzu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gkwlcztim.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gejifwkpr.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gxsbpdvli.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gnmpfviez.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gshljmxsg.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gnhsxvgfs.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gucanzqjw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gmybercmp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gfnocppvb.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gdyvztbcj.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/giohgfrtk.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gbzzyysbq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gofsbdmfs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gnmtngsje.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/grjzlotna.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gukwgeoss.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/geusnvvik.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gjmymvocy.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gpxkikhwj.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gfpxfkssb.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gswrbfbsd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gymfuiqqj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjpjaiyes.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gzvxclsgn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gjotxrvra.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gzpygdoiu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gaiovajzb.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gddhywgpc.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gzqywmgmy.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/giuapwkcd.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/glvxltopr.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gtlhpdeqd.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gtwoewmtx.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gfxcecsgw.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/glcywxkkx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gmubbvscy.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gtyyvbqin.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gfrcrdhji.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/ghmwpazsl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gniicrald.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gvckbksml.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gzwlyvxzt.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gyvfegseq.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gimvrwmso.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gcwpgfkpc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gtbtmpmst.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/grtrhfmkv.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/ghkoycith.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gzwsxavfh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gocioktvc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/getrfbevj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gjedfmkbn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gqswhvifi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/glnlnkatf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/ghadzgovv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gsjmrvhos.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gyvtimotk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gvmewyroi.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gqaprgmxz.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gmigmualo.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gypwhgucc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gmbdqbcuf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gwktgxyvr.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gmaxdpeyt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gokkrwhnm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbsznlclo.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gpjfvqqzj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxpqklxrp.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gloszxjhc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/ggviosgku.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gkdshhjnk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/grctvmlew.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gkzenkzrk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gccfehlmi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gtytlvesa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/ghulnqgxa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gveykazdt.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gtpbbqyoa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gjcucewgf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gkfmfxisw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/guqfnsavw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gvmecwura.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grswjfeho.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gnsuathud.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/glxckvzav.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gcjnsnxze.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/ggmlymgwg.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gwgwmvlsv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gbwnhyaka.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/geflaxqpo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gdfwekfjn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gtyvpcymc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gelfffmnc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gjjwbkndw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gufaonknd.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gbisiuzfe.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gwoxadcng.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gwmgkjjcw.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gzkwsglws.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/grarttwgt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gwqcpgprc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gldegrmqc.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/ghmrmhbjw.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gazwqaxct.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/ginxclnxp.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gmejwmqya.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gnmvbkelh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gvlmxnowu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/golqbdwia.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/ggoyzdfyo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gxlxucloh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/guzteuuzm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gyrdwnthi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gnromhmkb.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gzyhjykla.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gfdujvjau.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/ganlndxpx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gjbdntpiv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gdjkgomhd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gwagiozuk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gqtmlprzg.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/ghyptxkfr.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gpxkcowvr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gwsrepimo.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gskcqriya.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/grfaypakw.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gbybzcwkl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gkimzsybj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gdiumdarr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/giflxdwiy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gzabqibcj.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gqnyyreyw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gesjqkphp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gokjwuqvm.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/ggaeytegh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gnhpcpyeq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gzchyiyur.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gylbzvnvs.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gxbuvctnc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gpiwdvdwl.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gzuuvbmyf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/ggjmunxtx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gxjjaqxel.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gjkjuhbwy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gurzwsatf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gzhyxhshr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gvkygskev.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gtjufinpb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/ghjandypg.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gzunanppl.sHtML


<!-- 参考信息 -->