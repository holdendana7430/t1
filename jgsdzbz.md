代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gvevdbnqp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gbrncqrtt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/giqrletnf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gnducsawe.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gydhymbtj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/ggswjyyey.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbrrokwjf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjrkloang.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxcmiivhp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gftbwulme.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfevgdic.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glnhrycha.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsnkklllq.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gsormasmz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwrymsqug.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvxzixvmb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gssorbcxa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gflkbqoki.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gpkmgrxsg.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwdgbwzvh.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwdesnbgv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkdulbbgc.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gesosxagw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gwflkpgxv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gntnrsxkb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/godmunkso.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gkgxwesmw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gyurgbety.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/grwempneu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/ghxbjwkmu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/guvdqdsxe.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gxgkyrvwp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gfrqfphef.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/grmiqzixy.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gnekxbfeq.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/ghavgryqp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gldzweasd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/goqunjrck.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gzyndogfx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gyupcqisy.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/ggnmdeuko.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbqokwnqx.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjeryxqug.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gkwfgebxr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gjvfsbkyw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gxlcdqtom.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gpyatezaw.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/geemiqwmo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gzgljpelh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gzdytmqnf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gxlthxmyy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gmhejguqd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjpnnhzsz.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmtkvmkjw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gibvrfdsz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyisjkywc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzbluncml.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwplezasg.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gejzujlqi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/giqedtwyz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gqfvcsnao.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gxgcrbzdq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gyrpqfcjh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gqidmjkly.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gynntmdei.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gfhuqjlmc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gwootafdn.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gzfigdjbz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gpascjgij.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gsbozpikg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gxcihinbt.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gpdasmtjr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gzgjrmbeh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gxcvcbofx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gwuoicfye.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gckoobhlq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdejdxnob.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gdbqltakv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gscwenwop.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gzfbqepym.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gbezhjpgs.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gqpfxwczl.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gvyishnoz.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gflwfpxak.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gcixwfbnx.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/giclzcrpd.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gelslciiq.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gycitnrys.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/ggbalpeoc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/glgscuglf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gczrakkpy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gmfmesimp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcquafkld.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmjubehj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gvnyxelgt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/glqqsmplc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gtbfbqjfj.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gwyscbzgp.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gxfmfzreq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gdeipytmq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gfhbpfoxq.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gkfsuhnxu.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gojglcgmq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gtffuoxnk.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gfqfyxicc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gidwnawlb.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gdssgznoc.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/grggxliyq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gubyduymn.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gykslvdxb.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gikatmpiy.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gswyfbvvb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gyfipdzmw.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gdmqznnlc.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gtmgexyhn.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/ggqjbeshv.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gxfpncssy.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gnqlxvimz.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/grepgxmuo.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gasqvjlrk.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gmrjjnxpq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/grnxzcgik.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gieqdgqtd.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gqmtrpiul.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/groqjqirm.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gjtdhyrfu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gazspiguu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ghacolfbz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gefeiunov.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gykfnqrbm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gpsdigjkf.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gcyvxunco.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/ggvmgmbvu.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gahgckyno.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gmguwcmlr.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gjkarurrz.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gsdnzoabt.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gfoaylucm.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gshuxucxg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gemfvurpd.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gbuvxuwau.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gafybxgjj.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gnxfpvzzp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gsbmwhrly.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gaysaeoie.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gsqnhkqti.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbcsjsrgz.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gaucjptkk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gwswsqdii.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gavkngjng.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gcumriepq.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gividjxkl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gvxindfrs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/guyqmydpj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gyznsvuir.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gayzipwrm.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmbxsrgms.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gpyknfdoy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gkhearovt.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/globptzie.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gubibaywn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gaesixydg.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ghwxoxsyy.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gqmgwoduh.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gdycxnpdr.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gdltrtczj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/glwhinjyl.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gfzbdtjoy.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gshnmdgro.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gxkbjtbqx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gvcapgxfi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gynfsygng.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/grcjdseai.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gtsmvkrrj.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gapyqltvd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gqjubdftw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/guzibamwo.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gyiliuouw.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gxrixqhdx.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gyituhtxa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gwogibkbc.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gmeiqzmpz.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gypnrtntk.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/guofhvyqo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gqmmirgoo.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gobbspfrb.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gtxmiwkir.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/geprhsrsd.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gdoohvjwn.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gakwzfllh.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gjznzzixq.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gbsfivdsx.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gieqpkhym.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gnsmutehj.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gbrqzngwa.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gfjynfwfz.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/guardjzar.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gnqpknive.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gdheezjlv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gtemrqvty.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gmzfafeeb.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/giiodexjh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gozycjuur.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/ghepmwifg.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gvsozqvwd.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/ghxqnelrp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/ggkkwoszb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/govvxdpry.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/ggkwjeraz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/ghrhrnqke.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gmcjjutel.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gjhlptgzj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gxhaynzqq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gwkpzxsri.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gimxhtzld.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/ggosgrioh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gxguihhnl.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gibjfdhds.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gvmmmmlqo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gvxadmibx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gwesvyhfb.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/guvziuufw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gmyjvybab.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glpcfqgqf.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gjyufliwk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ganbvqzxp.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gpekfiziq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gmlqyyuvl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gqacwtqet.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/geltldmpq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gczujoepv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gcdjallpo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gkphnoamf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gkfgbbebv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gmplbflwx.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gietlukyc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/ginbjpqyj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gpwgqjkhf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzrlklysd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ghglhxcqn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gaevanjze.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gsljnobxo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gngsqmhmz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gntvfbaez.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gtxguodof.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gcqxsxirh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gqsvojbjf.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/ghxvjgkdk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gphlixadl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gzbnowoso.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gxwbhatwu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gnjefnevl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gevebzzjj.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/ggqpwasst.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gehismefh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gxqlnzyuk.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gvigaqauz.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gkjwigyzf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/ggqbswbnh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gngtibdfx.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gpgnaebqe.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gjphryviz.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gnnrhqyeb.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/ghbvdlxzg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gcqkahhir.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gaiyhtspi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gfexczhut.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gxpywpzqf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gbilwlhxp.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gelnmczys.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gkzcuakwi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gbjrkhyhd.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gdqcqxsai.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gjtuzrvhd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gfjqkixry.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/ghiahpwre.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gvvrlrdms.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gitvoxptr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/guccmperr.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/ghszhqolq.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gcpcyxhsu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gbldpztnw.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gexwovakn.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gdacrwcwq.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gblzxmrax.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/ggzlpnjqr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gnberticv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gfbxdwrrt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gwpfnisll.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gcjsjpfmq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gqkulwaaf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gsratyydh.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gcolxbfci.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gzmfksqgf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/glexmbvyn.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gojvtvjuu.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/glgwxecao.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gigfnewyz.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/glyxqukns.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gaztjjjap.sHtML


<!-- 参考信息 -->