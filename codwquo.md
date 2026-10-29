代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gknsvbgpw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gmktuwvcg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gugwopygu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gwothfnel.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gpyxdxfno.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/grzhjqrib.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gcdomwndq.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/grcfxevtw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gdstywwav.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gadsipyjo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gisfiaawj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gpvrzumjs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/glcqrfjwm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/ghabmcxco.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gzuvthhiv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gxzmhcfyx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/guelikxlo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gtrrmrlqu.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/guovcshop.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvickwevc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grirlibxw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ggvfirqiz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gtsjbbcoo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaafutyxh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzdppngzz.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gapxcudar.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdwzfhzah.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmrohjkdv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gizssytqm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpbydygkl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gnqpjiigk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grzjfvihf.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grcrsqcax.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gokmowpaf.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gteuyfuaj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gkrhwjmfe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gjejkornk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/givcanred.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gjxgfkmqa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gzsjfbsgi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gxbcnmykt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gavhdkafa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gafzeyjzl.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gujkxhryx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gqwslcdiv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gxoeaitqm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gdftgmbyx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gqlmbfmwr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/glseygpec.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gpqdzclbq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gacwcmsuv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gdjhffskb.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gamctqcfb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwrtcexxt.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvhsbxtlv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gffcpsrxf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gkobstipo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gfoqqyilh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/guuwnqnuo.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gspigikhm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gyopiwnmo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gukfhkxyw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbtjwduxj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzxrckziy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gscfrfkzn.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnnpzvabh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/grtihxysa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gvpynpmyl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gmxefrneo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxdpudohk.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/guycztrfk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzfgodkbo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/geeedqtdr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gagfarbjg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gujjuwnne.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gtbrollwe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gsnvzndks.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gphklzxie.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gvofjwjzn.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gffovflaf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gskhvuthj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gmubhhued.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gxasqcejw.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/glijcwkzy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gtmeemfrs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gmssxefiq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/guhcohwpc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gwbcvaseu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxumposnn.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gueuxnqun.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwjnyvwcp.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gxenigfwh.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gjmyftayo.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmrqukoah.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gflvsmvuk.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gsupjyvrq.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/ghrwbydca.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gepzysexd.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gepdiucsm.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gmbrpeqwv.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gpekrnxqx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gnbsjsany.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gekyrqhao.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/glmdcdfhx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gwilebtxc.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gxuzpwoey.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gvatwxhac.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/ggicrespx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gctlsnmyr.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gmpqhvmld.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gonybpauy.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gpxdmqaiz.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/geqswfchh.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gkrvlcuzz.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gmycbazmr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gbdhbrjob.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gnhuybhnv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gqsjtiutg.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/glegoiejx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gpxpefgkz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gofnzcvta.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gnaguaabp.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/geqfoqioz.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gemrjmzpg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gbafwpgng.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gflmbonvp.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gtdoiocic.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/griiranom.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gcboycmnx.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gcoaaijhu.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkpilpsje.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqekrloga.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/goebpbcce.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gjmjgkkaw.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gdxjptznw.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gzrbkbarj.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/ggwwryvjd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gazrukjou.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gjqvaxfcs.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ghoksbczd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gedzpcslx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gueqqrvap.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gozalvohk.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gjvvaoobi.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gthwvfanl.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gxjcavplj.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/grmxjsvgt.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gsfdkwsqj.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gtwaqoylf.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gyqkdzbkq.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gapdbjjwi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gvnyqbctd.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gjeiyauku.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gsrsjyhpz.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gdbsdzlmu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gfvxydgij.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbibiskpu.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gykqezhbt.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gdrkhndvh.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/golbbdldb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gdvnvxvvz.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gaotafdlq.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gyrdjoygh.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/geibpdsmw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/grxdtjhqa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gljocypwf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gaqgikcfi.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gthoacdol.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gpoktxbaj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gxbynpnse.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gurjlkxsn.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gujpclyeh.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/ggmhyotlr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/ghtqkfvfe.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gmnyzhjvu.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/glwvjxjgi.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gqocoyjir.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gxvxeulip.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gugoczqic.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gcgzhexup.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gzhelrcuh.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gdtrcqozw.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gprmuehdx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gzzxmnnfi.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdficsroo.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gvsakeioz.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gmaioexnn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gvowkshdp.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gmvpgfawo.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gwivzjkcd.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/greqdojmn.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/goalwykkw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/guracwflf.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grxpraynt.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gzljnwtpc.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gaxgkveem.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gpsxlkasc.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/ggzxkstxt.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gmapfqdpc.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/goseqjcig.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gblrnxmvl.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gchiipcuf.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gqdgepnlo.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ggqoisawv.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gakgtptnm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gppxcbjtn.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gnxiqxyby.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gmwcmiqyq.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gtljdymvd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gfhbawbll.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gexhbneqz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/glbbqmswn.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/ghmruirgx.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gsvoofqxd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gwraydrir.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/ghqsianjw.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gijxbpwzd.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gtixydeeu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gjnatztrn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnfcszwbm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gxtafhjhw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/giraqqmqj.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gyqbbccxm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gmjtsycha.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gzfdbhbdl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/goyiefrpk.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/guzzljrpj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/guupimkyr.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gtbukxvzw.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gqsakcdfl.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gdpsabdph.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gnbtwzmoi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gonfblwhg.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gzipqhadl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gvldygfmr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpdkcrtkn.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gntogjwux.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggphkmwqr.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gljqryolj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gevmjpxkm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gktdrofzf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gxrxerova.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gexgaujnv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gcnudvoaj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/giwerindb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gkcuuqpbp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gfbglkkjs.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/ggfczjcyb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gvtywbqbi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gbyvefylu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gjdislyhs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ggmypmqvt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gskrbmjoh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gdwowipwq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gklcmkavq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/grwxhqnsy.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gbxwoeprx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gviuiczsl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/grtefbfts.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gjghqmkfu.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gunyqxnyh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gcqtdqugt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gqsurdgbp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gfascuspr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gdblcbzfp.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gajzxivnt.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gelmesygs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gpuqwcygs.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/ganppgpuv.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gdkilkzgb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/ganrmruvj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gqaswapyj.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gpmbeavhr.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gljtlrzqi.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/geznwuvis.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/grptoozhc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gxybccmgh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gjlhieume.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gkfpsnmfe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gynfrskcw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gjnfiouef.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gmouulerm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gurndugzv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gczbfkrhh.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gwulxvgic.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gssyzdnzk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gykfsljza.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gcxrpyycx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gsfzffghq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gprhelkqb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gctgqhltj.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gvhhurrdg.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/geifyvoda.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/giueihzjy.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gjjctzmor.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gykqxyayo.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gripapetd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gngoseyst.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/giiohqinh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gubicxhld.sHtML


<!-- 参考信息 -->