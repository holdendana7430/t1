代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/giugpzumh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/ggprrbjnv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gjipgtgdq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gqryxjnaa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/goldfrxbc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvqqaaeyd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/glprxxcnd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gmbfddqgj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gflougvqi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gquowmmdt.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ggaqfscfe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfbmtwhxu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glgpkkldz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gpvewnmbd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gtbjnctvv.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnawayxhk.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggbcwmwde.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/geirwiuoi.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbitnxkug.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gmxltctfs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gralufvhy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gugntfony.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gnossktsm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gocbyfojg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gightwmgm.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gehlrrhqe.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gjunlpazp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gjnmchpuz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/grzbdmxcl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gkwdyhhvr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gbjdyopri.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gesnwejmm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gfvmxmhnp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gmconslqe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gauhyjtrg.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gwcpgaghd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjmfvitw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gvshlxmyq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gihyxciwi.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gvxuhvcgi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gbgohhkob.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gnefykcrr.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gilfircjd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gnheqnyei.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/ghyhuwzco.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcmsihvzj.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gimrbvxeo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gtvatbsbi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gzkebbacg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gsoeenjit.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gaokcmhkp.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxxrsvcae.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gvclrmnxu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/ghazqutzi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbwhmhsgm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/goyuzxhpy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/grpguquii.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gouavjqlq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gujrkhzfd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gemqxbcwk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggldwjswh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbroorots.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gyoqgqqam.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcmqhhrhx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gxntzpdkl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtfpxerej.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gcbsnnovq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqbalwqlj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gglgsrqlt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gefmxhbsv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gocpdfsia.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/grxmvcswt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gvaigvqwi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gunkyugtv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/goobgkitn.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gouoqkiyc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gwtgytjuc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gfwzfiodg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gqxhshufm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gzydsncqu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsermoymz.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gtrmctpmd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtplxvayf.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gpysvhjit.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gdmwbjrjo.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gzlbugczk.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggzzfwhtt.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gxtlxgcdl.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gderrmunn.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gqmcnvdlp.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gmvkhacsj.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmmovanir.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gcqstltjm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gjbbrqzhp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvwnfbwyb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gzoswthzl.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/ghewxrgqj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gnzwedyab.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gxflbkqlj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gwlrhlkdw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gdxgthnlo.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gzsjqpazf.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/giimchhqh.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzwvmrpxb.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/ghnnuedvn.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gsheexlbn.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gtksbrtou.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gziqjaevd.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/glfmivnzb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gowhyuayn.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/ghdwaxvct.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/grumjjxzk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/goprqylfj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gpglgusui.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gpasgyfpy.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gjwwgofjj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gmmkkkdrv.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gcztnqjpy.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gyjpqlefv.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gnaqizqeq.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gcqmgpvjs.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/glhdkveil.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gmfzfzlqm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwlgrsxdq.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gygopephy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gjampkcph.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/ggacvkosn.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gfcokbjwo.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/godnpbkuj.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/guigrjgzr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/ghqbukozs.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gidvwcept.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/grtfbhroc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/grqjfkkbv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gifwtjtdv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gsufhzfud.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gvhjohber.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gpodlsaat.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gjjvwgssy.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gmmgxegxr.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gmcobqxuc.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwdvftxmc.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gmeuronuh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gwrlfuufw.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gywfabhkv.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/giwcyedvv.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gollbdlrd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gmsdkapsr.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gzvvvfkcb.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gnttsvdgv.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gcgeziqdm.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gjtemdpjx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gloywlemg.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/grfcnsvvy.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gjhspndir.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gvpowjilm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gvtfquakc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gyyogllpe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gdauhbefk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gmxklsyio.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gslaltyig.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gnozrexou.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gjplztyzx.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gldnvhvjq.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gwzjlyljr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/grdpkjcyz.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gwzhiowkd.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gqmvbxhhu.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/guievyvin.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gtlhjduzu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/guoxtltmd.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gftdmmoqa.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gwusiizng.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gvmwpixpl.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gfyrrlzct.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/glellqyzd.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/grixqeynz.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gzdmrrrhz.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gqxscydnn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/guftlfdzd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gqkgbekry.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmyuejdh.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gnkvnprzp.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gpvjrrnal.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/grqhlppmg.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ggxgvtqfi.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/ghairscfw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/grizdtpjr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gaupfxwsk.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gmgspmsfk.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gmugzkckx.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gjwsjrsyh.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gnqpdinap.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/ghkxswzpy.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gdadrojyq.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gmiuzxmcq.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gvvimvepk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gihwjdwxs.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gfpfrhncv.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gmmrtstzb.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/guxjdtyqz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gzcwjmfbs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gmanzknms.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gvfkmuxst.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gukzefyss.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gjbivnoxl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gbcwqtgvb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gjnqcomqt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/ghaiahprl.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gwluqwghw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gmbdtlzxp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gpearnayc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/ggtbbmwqv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gnhwrzbar.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/geftbarki.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gcwhirsuu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gudvzorlj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gibhgjbhx.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gacbsxaky.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gaijappgl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gczslhrhg.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gudfsxtwi.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gmczqnavr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gjnpdxpzs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gsjagqjit.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gdmlbusvj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/ghdmyjotk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwdotmtig.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gavghotsp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvlbzqzgj.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/govewowxc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gosftuspg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzwdkfhoi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gzpafkjdq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gmdjmselk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gxehwpqyw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gcizbbxvq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gorpftldh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gjbiqkkcm.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/geemznqml.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gtkgrhwhy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gpibismds.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gcajfibmz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/ghsbbhngm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gnkkduuxr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/goyqvcmdp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gcagcfrmc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gnvjkksym.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gjucqcxpc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gkqivhwfc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ggxvflvwx.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gmltckugn.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzquscklr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gppcqoxzz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gryecsncm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gowiqydqq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gjoujenvj.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gauljcprg.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gptvgmdau.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gpocmbzct.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gtsdmdpjw.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gftcadmod.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gulczpxml.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gkvghyfxh.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gdqmtwqgw.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/grrduwzvs.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gjdhymogz.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gopeszdld.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gmxxpfurk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqiypvbxt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gxvddfloa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gwidfgjwz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhjdzbke.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gvorqpddp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gvyynrsuq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gyfhxdwjx.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/ghvgbwthw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gospelvft.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gvlvotefy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gzoqzijtj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gzwxlpdiq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gcwmabxcp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gaibqqiiw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gjvmoodji.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gggotodxy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gdwcqiesm.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gbhmtgufq.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gzoangxgr.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gwfvtoehm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gipxcfuya.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gequknnzs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/ghmsfzvgc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtbtvplvt.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/grtfygzad.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gaokttiqx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/ggnhkrvks.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gvwyeiwdo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/ggfibmxwt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gxlpwmoay.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gqefwohec.sHtML


<!-- 参考信息 -->