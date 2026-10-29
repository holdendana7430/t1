代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/glnobpqmq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/goiqzcjsy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gmxxcviop.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gfstqzeow.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gwandokoz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gezcuzxky.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gfctgnshv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvmrdfzig.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grgcrvjql.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gdzuksngc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gopycgsqq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdsdgqbfq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwmynwsbb.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gaqejgipf.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcwjzjkiw.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghpszunzx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gycftwtti.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmjtwyjjt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gbgnuhgok.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnolqmxvf.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gurlmbxga.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gpwijczuw.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gqapznolb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gbwplwixw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gsyybprmm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gktcipkeu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/grusfpnni.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gxravogoj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gnbhztvxx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gczrxyefi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gmwmwubpz.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gzpksdels.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gnrldlfgq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gqwtedzxg.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/glsagnxza.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gbblhpwio.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gzzxonnmb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gfbyyarjx.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gnpcswfiv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gslabmuxr.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gkkosatdp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbtgzjekp.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gbhsxmbrc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gzracovge.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gqlmhhohw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gzgaslpcx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/grccrkzct.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkysrjxqs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/geuclcgzp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gexlwuebz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gccxfniog.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/guviznmmp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gbtplypdn.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtugtudnm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gcelmuozi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gjxctscam.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grxkzbmoc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gagitmmnm.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gevckhoif.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtrhstnes.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gmtbptvlo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gajjieslw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpaabwxnx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/grvecxxew.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gxelmyvei.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gudjmioad.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gepiqjpyu.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/genxzkjxs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gvirmpbbp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/guvbmccvb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gifyzkyjj.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gzlppqvui.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gqyzzxriy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gcpujtcmv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gvtrvwvwj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gkngcystv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvmrxgpkb.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gyblkbtva.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghbwmmfmy.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gkmbyreaf.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gkbqrczec.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/getghzbbv.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gaqnshpup.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gtmysbogb.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gfwlhvecu.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/ggmjwyrtn.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/ggxalfqdz.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/grmzsomzr.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gffwypmot.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gtweckthx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gbhqcxdqv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/glxgzbway.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gpdnkfxub.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/ggmqgquka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gkznnqcbv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/ggbyabhdn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gblbvgfjd.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gkuczsikz.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gncnszoow.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gqgnumbua.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gsxaqiwzx.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gioqpljth.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gaudfnkoi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gcstvgjbb.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gplxgxmei.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gvobimiyl.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gaizkvoly.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gbjsufpmf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/goiliaibi.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/giixnvdlv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gfogonupl.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gvlridamu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gqfskiqiu.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/glnhkpgrn.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gxwrfqbbu.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gxdgbdmhx.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gyegkbwmz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfttdfcgb.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gapptepth.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gdbdalxgz.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gkmautjsj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gkxukiuex.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gxdgkofbp.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gnhtghydi.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gxmxxzhpm.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gsxdxeort.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaiykgluf.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gmfwoakjv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/grrvsemvl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gtsbnoljn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gtfsyuaii.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gniodrzzf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/goyfvslch.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gmepgmtgw.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/grmscnaoh.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gdqtitexu.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gmptbucra.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gpelwzycw.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gjaexiwzl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/grvdzcxge.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/ghhezddjr.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/ghbwxigyf.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/ggzkncxrn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/golqjoznm.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gaojtgusf.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/ggmuekrmr.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gknoanppp.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gyrtiztbw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gkicnvhtt.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gccqzwaqa.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/glesncvrw.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gimnorcit.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gachlbhrg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/grrqbsfjz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gsybsipkh.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gukiwehvh.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gjsfkwvbp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gagdfffgg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/glmmgnqeh.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/ggpjmkyoz.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gvdhbjjwm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gxstpinez.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gdhknruhv.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gnjjifpin.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gfuxpwjsx.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/grtljossv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gcdmlahxk.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gglgczalt.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gxtoodwst.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gnoheepaf.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gsmgrwhrm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/godqxjkpz.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gfndeotzh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnulelqcl.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gxhbbhbze.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/grmilgyij.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gbymqbeoe.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gnjwwopga.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gchvclkui.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gvxnuqdnn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gdvrxilps.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gverynbuk.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gblxfrdxm.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gicdcpdbd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gfwjvwzqm.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gncwleeic.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gdpvdpgas.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gcnfiduau.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gwxcwdlje.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gvtbwiygj.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gxpbklqvx.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gneeaitgm.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqeeuxddx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gupzcayef.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gsqrdkkas.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gcxrdugpn.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gqbwqyxyi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gqinlljye.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gthshqmax.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/ghipgcyrj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gppfhhtsv.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gryojjouu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gpcihdfll.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gaoucfzhp.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/glzbdhhby.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gexvwokpd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gsjzjqwsq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gvvnxtncs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gqnpddxfi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gymnnsitp.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gbhkudlli.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gjrlrttxz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gftypvnic.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/giujtlvgl.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gmmvyjohd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gitmsnqjd.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/giidyfxwe.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpcheabvh.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gfywhsxdw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gvrtpcgmf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gnaemaivh.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gfnwagqgm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/givohqdpb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxbenalbh.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gpuuvmuwf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcnmnixnj.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gwzuzeyjk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gjiywgipb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gyvxducow.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gqgmueyor.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gsrsxhwbp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gsxhudlot.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/glzyadnez.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gpmdjsebw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gmeknoosb.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gokaasaor.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gotswkrfy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gapovbkag.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghzdnaxoq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gpsrnxfsq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtlcbtgia.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gqvxajpvw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gpmntwfqu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gfnbckoaq.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gfkhidqhr.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gmvddnhhp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gjcidxttx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gpdjebewi.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfuurcwex.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/grvaquhyx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gtzxolesv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/guqzjapzo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gobjjonnq.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/ggsazqcdf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gprkqviqc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gvnacykbm.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gnslxfdjr.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gfyuuxzea.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/ggtjmmvmp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gbztlcght.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gvqiqcgio.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gvvnqaamy.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gaikxifak.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gyqbqxefm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gkjqolelq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gxgeentvb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghyymugph.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gsquifuuc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gsriydhbw.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/glfzoxhci.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/ghbgbpjuk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gjdslfins.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gtndpynrf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gytydxhrx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gmzhuogfv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gnhuesalk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gpqlbjuag.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gnaybzbpj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gxjcipwyx.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gukgetwgo.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gpwkmjcqb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/grgzfaago.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gxtqbgxkg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gtusqqjtp.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gjunrbcwo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/ggydugjmi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gjgmubfnc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gzecuxppu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gtegihqes.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gtbxgdqec.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gbfwiaeyo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gkvimsyaz.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gfwlpqoxz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gvgepgenn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gdmjrupli.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/goiggqayv.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gnowleati.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gjzcoowvx.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gaghhcnkw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gprxvqxmb.sHtML


<!-- 参考信息 -->