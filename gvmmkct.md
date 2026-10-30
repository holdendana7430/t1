代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/ggcokptow.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gbjwfymvh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gkfounfwx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gndkljrdk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/glfhjhmvm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gucgurfjv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gbdpxebev.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gkxvgfdln.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gtqchgqrb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gzftkmlji.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gkxksqyps.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzecoldvy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqbnkjqjy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/grgjusjch.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gxwacevwn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkbjqinbe.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqdlwcdww.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gcuavsfcu.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjlkqyhuw.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbxencnei.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjaepspyc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gepolthos.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/giczjyhkx.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/glrewiqpo.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmrjpvpaq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkaquklhw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gvagrhgdk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gibqeukdv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gpzeoivmy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gscsgzbcl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/goqbtootf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gucbkdkne.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gjbrrjlqs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gtyqeqylp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gdxjhxdzh.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/goezibnam.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gpzldjgzz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gfneulskl.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gpppvxmth.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gwkdorkoy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/ggosfemyo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gvzjikwpd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gcqewpawp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gkybkmmhv.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/glaytvyyt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gipczyqtg.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpdakjplo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gctritglu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gigxoruat.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gtjqyiper.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gsamipynz.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdegmwbhm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gerrvnsbv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gcagynyfn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtosqnqdz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghzupszmy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjfhtdauq.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gislyhzbv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gxnldxupf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gdwkvsqnc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gevusuqwc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkrfzuhhu.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gpwogxvxt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzdzbxgrb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gtlwukqaw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbvmcdqlx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gczivbyyf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzcapzbjy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gvhjkznhp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gqjallosq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gwfvwqxyc.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/guxboidnk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/giginzvfw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gvznhrmfg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gyywrchul.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gekomuxup.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/glrdceirl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gkmbtjpiv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/ggypbwitp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gyqcwcxyi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gccbjself.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gdcotcuxo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghklpnlmf.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gctsybrik.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gixgtxqvr.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gemebmqzt.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gflzirapi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/grjbidfuy.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gcenhjcih.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gvfrmxafu.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gsmumqptx.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/grtzedbyr.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gzukvzwot.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gmvicnhxm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gjjdtvncb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gbjfcevjr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmghdepnv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gutllwdwy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gfspmghiu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/ghpawymka.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gxmpbjgwv.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gfwtzduap.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gmgyrbroa.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gexzyamol.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gvbtorrqt.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/grdsmzeas.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/goeovhxer.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gjfokqocd.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gkzxlecmd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gabwjmflm.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gahbatjaq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gikilfigi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gvnzpsotf.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/goqrgcdjd.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gfresmhck.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gfmxynaej.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gpswwvsro.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gstkiyhmb.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/ghxvlmkks.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gzqsiceqj.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gsyxntapo.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gcmxfhmmz.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grkdnkeyd.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gnhtyuswm.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gfssqmhlu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/goevusfwa.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gcpwammjc.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gmjshestd.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/groestjlx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gyplqpzne.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gjnodksea.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/galsgqghz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjuacvpid.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gevamukco.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gsfqkocwf.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gobcapapg.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gichouhyn.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gxugijxge.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gaxrwtwqt.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gcdlhjarw.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gsoaxpdfq.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gjijidlna.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gmzuacpre.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gtmezrong.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/ghwidilsi.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gvpxjxgxb.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gpbivgrmb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gycbyiwfk.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/geyzaxago.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gsalmkqvc.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gznoubqvi.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/guyqvqljt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gdngjalrm.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gdgsrpghl.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gqeozgogq.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/goocpurpt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gcseocqrm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/grqunizdl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gaexrzztf.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/grtjehecz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gsujyvryh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gvlazczzf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gdqkrkmyp.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gqjshjfno.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gsjpbzzqd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/glvktlfjc.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gwfmanzcs.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gnqtqdwmw.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gexuezudw.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gpywbxaoh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gegnfjzqe.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gollsllqr.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gtneswwrx.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gzzhuetff.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/grkaqqpqx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gezdvyejc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gfybhmvib.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gumlnttuw.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gtdkozgze.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gwpzhdpwv.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gdxlmzbuo.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gbaoidflc.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/glybrapwh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gefecnmnk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gvpkemngs.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjglyohda.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gmovfrtyf.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gcpvkzlvw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gtjmryxvu.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gamyfiebb.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gtmvgyfmu.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gfvqxuzmw.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcmrprag.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gbdcyeigp.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gjvbkhkyp.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gcsvdwiyt.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gcflkqohw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/ggfembydg.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gtvoixnzh.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gpuwtqvxy.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gbupuisiu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gmijrymtz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gxczqcmey.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/ghbcjyrem.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gqrgskgxd.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gmajaiwrh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/ghazlrjdv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gpxmmnzxq.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gevlthred.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gvewbvbze.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gqmwbsjzb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gbknsmvzt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/ghrxdmpdq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gdzeopycd.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gycrqkxpn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gaajwnfoa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gfowxkdpc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gbvizzebu.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gdvhhxakk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gjfonrxvn.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gcfszoblj.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/guisqgskf.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gzjtsdqic.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gunwyjrhj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gxgxauuro.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/godqvrlzp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gbrynjwiu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxisnwnee.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/ggwrxiojd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gedtodzzl.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gqyjciedj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuaylnsz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gllehjfie.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/goiruumfm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gdomjhrix.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gytpbvtih.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gjrrxxsla.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/guisqoclx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/giipabdti.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/glljmspiw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gyqudiheg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gbmmmxrbt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gnfxgwdys.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/ghyyrbmxv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gojxckwye.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gfonzoesd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gcpukhhtd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/guoekoulj.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/ggpvewgcb.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gjhblcsno.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/glaxykjfn.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gbodyrldm.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gopyhpemt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gmarluilx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gbtaxcbjx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gcvgziboq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gpdkmhlyz.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gssksvnml.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gqsplytko.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/ghshngntj.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gkvfhraqe.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gxwtcfidd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gorbdgwtj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gecftzmfx.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gkeihcdnr.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gbewlbzno.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gkufkyusx.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gnrlvoiyq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gcxgjwlfy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gbhqsaoqu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gvhejqcag.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/goulgjnub.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gawxldccl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gipiqmwed.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gpvjajirv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/ghowpwgzb.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gfmxrkzxs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gfyxqiswb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gosseztkq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/geqmhwcwc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/ghagpxtcx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/glgzfpmqw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/geexgxkon.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gcwqmbqxf.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gzlzwhrat.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gydythzvr.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gdmmcbkqk.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gsxokpopw.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gqrtirmst.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gmeqdztse.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gybztiycb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gnwxthuew.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gcsvpyuqv.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gparyshrj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gktumuzoi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gpmlfyxcu.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gfgitzjeh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gkviyuzea.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/ghtabpfdl.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gqqjwreys.sHtML


<!-- 参考信息 -->