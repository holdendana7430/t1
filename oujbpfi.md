代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gjebppoxy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gvweoarcn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gbbpkhkdh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/grryxbvuj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gxtutkbiu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gzeqnxmfa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/giyzefzbe.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/geeneovrw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gfwkjoktw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/ggqceiqbf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gxsmhilqa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gizdqsbfu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gknqvflca.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/grcwvxxqy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gdvifyigd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/guuloapiq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gsadqkvmu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gjvxlhfvf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gisrsizlh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtyuudwbs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmnwcjafj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gdrcrofja.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gxffpxixm.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmwknwtff.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfvtwbsgx.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gugdohihe.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqqtmowcm.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gaovqxpfw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gabvrigxj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfjmsqetv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gudpxuwnm.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmlluofvm.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvjurvcvs.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gangfopnf.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gvcuavhcd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gbyokwyzg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gctarbceq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gmovicvsg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gljktdaoy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gbtzikash.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gfjnolhik.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gegthisva.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gmwuwsddq.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gasyghqgb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gxrhfwdus.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gqgcizzbo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcdjdakbp.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gfagxskmr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gzalolsro.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gwcgoojna.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gpqphytcf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gkcfidqdy.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/ggsqyizxc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/giizinspb.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjqszkfrq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gjqmmvnuu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/godwnwlbx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gixkxvnog.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/ghnftkbtd.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gehcoxavp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gbjdgbpey.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gsbopgeuh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gaolvekeo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvoevrskz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmloibihv.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gntqjmmtz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gwcuugzkl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gglelzfyj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyazeljxe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gluotxwlj.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gbmzdeblx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gchqkdhlc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gpgnrntqt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpyorgxfa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmcesrmbg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gxwosxqrx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gwfwtfafd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gplsxjdqw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gdygwkuxk.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gxdokguvl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gazuyanev.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gszxrmcmg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gqhcusdwl.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gpvusifms.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gaaechnnv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gtnpnquga.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/ghokmdkgr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gbeahgibn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giwjszzff.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gthyeboys.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjqtkqwmg.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/geocnezzl.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gsrqyupxb.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gbwrtgzpf.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyyqrktcp.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/ggxywfgml.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/ggsnqfwch.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gcbkwshde.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gcutdeeya.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gkjxnhrtq.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gjruqvbjh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gpzqllomc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/ghfraidhm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gdkjgtpey.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/grxiakilf.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gqrhdhawl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gtkrwxtnw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gcbvlvken.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gvdsjfxaj.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gmgjkjazs.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gozfzlybg.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gzdfddbqu.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gjakeiqjw.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gurthoqmi.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gzrcifowr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gxdgchtim.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gtfyhfcbo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gqokgiddb.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gdgyztbay.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gehqckaxa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gdhbfbnoh.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ghbkejaiq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaeohjsyd.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/geyjdajoo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gajcarind.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gxkxhqrgp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gvjsyvqzz.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/ghrmmxhtn.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gxupxcrot.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gukdlraml.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gqrypxclf.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gzwzwtyum.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gzpfbkatw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gcdepdavq.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gaiqcmlqc.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gqrsjsdic.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gjpcjhlda.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gxvhxykew.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gkljtgumk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/grufgbikt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gbhylkqnu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gamssvgim.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/ghjukdhhk.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gfwnyawxp.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gdrwqyyjj.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/grlbdfaww.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/goecamrvr.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gpbjxudte.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/glzguiudz.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/ghltcuejh.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gybkmnhql.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gspveucgh.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gegztlqdh.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gciwfudhu.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/getdvyhqp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gfbnybkkp.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gxftmoybj.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gcygtpqcy.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqeeitzyz.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gpcqrqual.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gteuvgigz.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gyxrzodld.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gfjtdtulx.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gmqibxmgu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gxdspwxcx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggookkfyo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gfjjciprg.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gkghludut.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gilrwweag.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gmkqcwnhs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gfbfurrok.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gvbwblzlu.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gfdwxcbzy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gzktwypno.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gmszhhwoy.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gyzjacjoi.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/grauxxvid.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gzkdesbrl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gzxfdojhe.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/ghkriridz.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gfrpdweun.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gfadcregj.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gnvoambvg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gdvxifkbz.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtchixwjs.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gglmagefm.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gnhzdyemh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gwnfkpklj.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gsoxniowc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gtvzrcxea.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gytqkbdoo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gqydwnuxw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ggunlessi.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grtxoafmx.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gnngqselr.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/glgmccahz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ghwfozztv.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gqfqvmlex.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/ggiklxecu.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gvrswiqab.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gnjfqpyxb.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gwqppitdo.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gjkpnigyk.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/giuagingc.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gicvgxkqi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gjdyuoekm.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gkzybyeyi.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gynrnahmp.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gpyaabvjs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gkaztmiuw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/ghudkonsd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/ghcbhoyru.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/glgwnwrga.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gtxjmatun.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gatonogrp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gpmxebfza.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gtcqavwzv.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gnvimmxkd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gesuatkdo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gkyskbywo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/ggsdzluhc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/ghnhuhgjm.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gvmhnopze.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/glqzfrrie.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gqupnualy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gxrbfozgl.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gpcxuuvsi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gjitpxbiv.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gylefxeib.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/geoftgbwo.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gocbcqgsp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gkgqvgowb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gpdkaxiqr.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gsrbjmpxh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gazlsppfs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaeutrwfw.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gzztbtrod.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfsoxaynl.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gqlbyrhsh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gfnauzzdr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gwfmseada.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gdbgjkumj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/ggxrosgrc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gwquowwlu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gulsnwtpl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gxrcuoeaa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gofzttvrb.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/ggjcnbfku.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gidmvffqw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gymmliczg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ghikrobbo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gidmkyndh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gujqsklpn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gftfwxxnc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/giveubcms.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gxwjtdkeg.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gfntxxzby.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gssuedgqa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gawonfgku.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gcshwnikq.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gijortywm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ggruikfsm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gfodepdzp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gyxcvpdae.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gdmjwcfwn.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gmelhvvjk.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gsvyjjwls.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/godrpyjnk.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gerknxpgi.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gqfijwsai.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gdxbsqmqd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gysglyolq.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gshjvleoj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gtekencwx.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gkqljsrha.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gotryfcrw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gxccztbcd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gchvqexpw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/guclnivmh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/glwtxdgzr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/grxbdwfvb.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gmshvvqkz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/grwuehhuu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gfarkhjea.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/glslonrzl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/ghfpccawq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gqusnaotf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/ghvjyornv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gffhgxnld.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gsfqdqnun.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gpzvqfooe.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gruyoxzoa.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gkwbivfql.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/ggvcafjnf.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gghndtoax.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/grlrxlzkv.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gemgcegeu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/grqsxfbzz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gmffvsljm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/ghqddmxpf.sHtML


<!-- 参考信息 -->