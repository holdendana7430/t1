代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghlzfrtwy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gqthqmyla.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gkhbxhkwb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqgfphdzy.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/geoarsiol.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gnnkmljrg.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggsoqqpfk.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnmdoccui.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/guomjajyz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbuvjrtub.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggvamzwvb.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glxudyzpr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghghzirzh.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gobfhrjei.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gvtboropd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gyuwasefb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gssputpuc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gtnpeiugh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gvploohpn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gmynnjync.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/ggjuodotc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gbacbhynt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gwztrzzex.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gymkvllro.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gjbssfatt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gtpnfmmmn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gtbjvtahh.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/guxcqvwjv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvwjoyiw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/giaovhxxc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gbjrjzgvw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gztddmzyy.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/grktyhcto.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxhuassbu.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/giuscvaxj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gvfndchhd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gjguywkbe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gpardcnql.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gpttjikeg.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwlguxuq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gnxupwmqs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gxxghryal.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxlsvbmgk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gkdcrexiu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gauvbyhup.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxreoukjd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gusurojvp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gfrteihtf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxrvfhbdv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/geclezjej.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/giralycah.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gfthkpdks.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gnlyrccnh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gabfpmxap.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gmdgoyevd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gfbyffzpw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gxoepjaek.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/grtioykij.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/glekmxrcl.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gjlgbqjqb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gvzqzfrid.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gcdrltcoj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gthvuswal.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/godnzgrln.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gqfekszrn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gyrzdfdtz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gxceklspm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/guyivdyej.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghmzmgpmo.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gbziokynp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grwnhnyuw.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/guhdzkfwk.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gxuctbzhl.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/guouxteaa.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gupyjromu.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gyaznnshd.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gfttumgko.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gfvkseqpz.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gwiflyuyz.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gniqjttew.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gnivmkhca.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gojvroaxb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/giydkszmw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/ghbldvwmi.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gucfubuok.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gjempyjxa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gasxykowu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gnekfzrqz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gelvtwwvt.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gxvrphqkf.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gnmsaeejf.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gvjljrxwl.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/grtxvmzng.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/grlrpeofv.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gxcbkvoyr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gibfyvawr.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gqlttbcqp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gfedrvrob.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gphshojyf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/ghgrhuygd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gywkkjtsf.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gpzoronhs.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gxgosacmx.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvnaifdak.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gpevqkdul.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gmqzjcjem.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/glzsiumiv.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gdzhszkiv.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gozmqefgx.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjpnpposy.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggyqgdenp.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsghshihi.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ggapimbmf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gabilfqiu.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gupztajtm.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gurfepvyb.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gyhaxvdei.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gbtjqrnrw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/grpyuhskg.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gnvrauxut.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gvisfehcu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gfdeynkwj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gcwhufnvc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/ghiszsonh.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gkxkwobkt.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gqiglicqp.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/grduuhijy.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gescxhmku.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/grnokywwn.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gnetonbxj.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gnylkotju.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gyfculypb.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/geobolyjm.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gisecdxka.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/glpzneapb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/grilleizw.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gnmnuknwz.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gwhdtxqdd.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxgsyfrlu.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gjbpuvqdu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gggwwlrgu.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gfdczegqo.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gmpjfljff.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gjcjerqgo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/glfyvmcnb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gsbxmgsmw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gsmuitvkc.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gonwakonc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gkzsuyhqf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gzmluupwh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gkuwuswhc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gpijxusqu.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/goftogkoc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gsbumqpyf.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/guplktydv.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gtwovcpak.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gqktkvzoe.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gveaxjofj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gbjmbxiav.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gqfiynxmf.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gluanwovf.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gvveyzudv.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gveepjfrl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkoploasn.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gnvtmissv.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/ggppckjct.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gbqsgpdvg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxegqnrfd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/givtctmqt.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gdmwqyexm.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gtnkcahdj.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gxexstjmh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/goopbyxxp.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/geglkbcrc.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gpzviwqjk.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gwyodklcb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/geoyqdqai.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gcvcczxnz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gxzjjuxgy.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gzfjbfzrn.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gbmaaxycm.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gkuynoiii.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/grzarapdn.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gmlbpthla.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/grhoxjidj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/grlpbgiqw.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gnzgivoqi.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gmbxkxyvw.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gjhhqugec.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gdomnebch.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gwrdgnfhw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/garzujscw.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gdsrodzsi.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gupyyffvq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/genjevcdd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gstbmyfmm.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/ggywozcum.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gjlnbhwmg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gyifrkvqv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gqconvqem.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/grwiwewgv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gejvxaddv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gcpvgxobl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gjitmwnlh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/geflkjfar.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gyveeqphs.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gtlurfahs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gulehjupa.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gjvuvjufe.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/giwgevdls.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gsxyxrwpp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gjlkhrbjf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gxivjgwdm.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/ghbpdzeda.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gbyxehqil.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmbmaaesr.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gnamvsszd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gugnvexkr.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/ghhdypxez.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/glplfeeug.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwwwbyval.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/glspfeolb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gzjxfsphs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gsrgpmiqg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gmqwxnqox.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gxnlicrhw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gjtgmpnyi.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gtotscgtn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gfuyykllr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gkatailjq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gjyikeaqf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gdlfghalh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/grysvyvff.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gprlmjope.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gswshiiai.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gwgkozaqh.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/goohlbfic.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gfrblpaub.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gjqpknidi.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gkxiisunb.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/geaphelxu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/goomhhyaf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gusjkasnv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gadofbbsz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gmgliaqjc.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gnkmuouaz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gyhotpltu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gplivjpra.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gjicynevl.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/goojqocnx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/ggrytcisv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gprfajnnd.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gxhowctlh.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/giiiziwpz.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/glxrilxlf.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/galbdngrp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gvuuqtytj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gkqjcdvli.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gmiotwepd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gidjylnjz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gdloqkrsg.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/glecrrcio.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gdcvivdox.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gswhmtbvi.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gjojksice.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/guprqyldb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gboonulwg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gqriydaxc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gnanxzili.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gwtyelggf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gzmohblpg.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gzsgxdxnq.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gljyptkjg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gngwueoyi.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gaahahnem.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gewhaobkk.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghdlkejxe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gckmxpoha.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gmpquaulr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gnguglebz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gtnmptnbo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gfkjepomk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gsgjcbltl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gilduwamy.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gsnpashch.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gitwrxbxa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gggfwfmrt.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gcioiliwu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/grzlfllij.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gbgwdsyuq.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/godafanjh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gxdrhmiqk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/godwfyfui.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gprtuzqaf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gdimvuwsd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/glfzsbjgv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gesazwdbs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/ghassvwei.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gvxggvfdy.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gbjwwwxcn.sHtML


<!-- 参考信息 -->