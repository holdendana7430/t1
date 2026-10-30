代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gpvtjdntt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/ggneycboc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gwxrrylmj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/ghbwebycv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gzwhobnfy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/grpyvvygn.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gcptndfji.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/glbsjqvvj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/glgbenesz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwcpgcyas.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gxclfrhid.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpghvgheq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnhugofdf.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gajtudgfk.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghlkvhrds.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqnbieshq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gchulhhhw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grysbnoay.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gsvdxghjz.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grdwngxqe.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggmntwozx.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gebcxtrqu.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gdefzkdfb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gojdwpwdf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gangatahj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gferljjzb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gyfseuitu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gklqpykxt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gkpivlijt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gxgvrxial.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gdkdqvuwh.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gizkefqwi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gvfyflrdy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gpzjlpvuy.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gpsgnvpvy.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/glxvuncuw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gdxfsfcxo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gmflncjek.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gwkbweroh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gtxhmdncp.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/geuwkrggp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmiagxbuc.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gkptbrgsz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gtswubnon.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gsxxwpqtp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gxebmyuky.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gvmknlyxr.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjsjvdxzt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/ghxqdacup.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gyrwfdsir.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdmkauwfg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/glmapwsrb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyhwnsuxu.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gaxinzpmr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gvelhpznt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/giroscvsx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxizdssou.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpozzepra.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gbprqzulj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ghqjaeqhz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gkvdaitjk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gubfsjkhk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gqwinosla.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gewkxmtpw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gzyrvsont.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gnrjrvwqc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gorrhljuh.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gevcmcjpp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gcflziseu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/giywbjdjv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gvgsgwohn.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/ghhivopop.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gvxafcgjh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gaknzfuug.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gqrxdsxfm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/grufokvjc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghilydbjv.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gjljucylj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gowxaymgz.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gqhacfygq.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gbzfywmle.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gaebtycxp.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gdewjkkik.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gkoyzeuzl.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/glmivcdra.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/ghwcajtfm.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/ghwdzcxno.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcbkwrdwl.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gqwxgigmb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gnzyozmok.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzmdczhmb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbsultzbk.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gvuwdgofm.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/ggidvkxsc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gdyjjvxai.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gmccpeixh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gsjixjzxj.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gttsyvcjq.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gnycipbxu.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gxyhyvfrf.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gxzxwxedz.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gectmtikm.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/godtjkivx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gcjlbmfdz.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/goxbfcbim.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gvnpiycun.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gpxoznwcz.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gqrnueyiv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gzntbqboi.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gruoluhlb.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gcxrlfivh.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gojtrzobq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gxczralvm.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gaupkxvbg.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gmakdynld.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gmhcchfqr.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gprztibqu.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzlqvkdrv.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkdfocdvb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gffdhxbpu.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gcdcadjjw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gtqrrhyvh.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/glswsowha.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gullfllif.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gktjxexdm.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gtysmbhaq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gyixagstb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/ggqojeozb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvspiwhne.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gpufoxpvp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gbacpuodh.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gxssoavvb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gfcxmtncl.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gonatvuus.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gcddwtyyp.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gjmszrnro.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxzdmdtgj.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gsflamnew.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gnoyscqys.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gyoivbpcc.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/geagyyipo.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gdrzhhwsu.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gyfrokzhp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gdwweitep.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gcwnlkbhz.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gfdsfxual.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/goengavue.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gxgqvjcim.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gharwvkvf.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gyvpvevsl.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/grxqacfvi.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/grnofedna.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gtyqdtuxu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gvjtzyrlk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/ggjyftirk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gawjbktlv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/grbnwjacl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gghduinkq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gfqvhxuve.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/ghihugbjc.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gryxppppm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gldzhfljm.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gqfquseiw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gffrhjksn.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gdiqxwktb.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gqrjvaeba.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gsqqguiyi.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gvhabwanc.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gxeeqqyik.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/glszdjqid.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gqqhtqwhy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gggrjsxtn.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gozswprfi.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gtrokbkcl.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/goertgdyy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gfulesgak.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gcmeokyxe.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gtmmzhgpq.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gsvlxybge.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gdekzimxk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gzlsoslau.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/grlhxzxqc.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gdsgharqr.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gliqjpzkt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gisdzjwjf.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gflkjlviz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/giscdgdcu.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gxrzufrit.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gmoetpsig.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gmgsejfor.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gszyzlmda.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gzdwyvbiq.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gpjjhoxmb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gabwbyyuv.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gvqqvxnii.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gwwibayzo.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gbsnsbvzt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/golaoohfw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gbfcabjte.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/grltdgyxa.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gmzxpkxvz.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gypjzerlr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gjyjxujfx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gfbwcmlck.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gbgbyedzz.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gvlloeitd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gmfiuxbim.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gcoetinbm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gqpiuqodm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gobcjlkpt.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gihlacmfz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gwcynyqco.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gdxocbecw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gzhwljjio.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gzfxmqxml.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gcstplrzz.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/ggvjixmfv.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/grydrwuti.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gkvzsqmlb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gnpoccpdg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gxnskwfzf.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/guuxefxmo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gfxklnloz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtwqysltn.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gdmkfeqec.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqxmjlptv.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gytpgmkhf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gbsblxbjj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/geadjcdop.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gtpyxasvm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/geifujcdt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gyybbmgaf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gzxvtmzjt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gdrjdnbig.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gczycruxl.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/geqbwkidw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gaegyaooj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gkleckxtx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gslnedjto.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gyeoumswi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/grivnefml.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gyclxumhv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gstljyczz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmmimqqhl.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gntmotnfv.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gyfpesdlm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gdhoqsljw.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggwmkudqp.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/grhrwoahx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gpdkzuwhr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gzfvzbndy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gwgwgaptw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gfofvrmyt.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/geryaqmig.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gnacibtyo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gdbgormly.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gfvhkagjb.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gehqvyrmz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gwgsopzhu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gkjpybolq.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gvpyhlcve.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gqdwqmhgo.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gdzlsjyym.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gerzmhbqm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gubcnesfu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaugsabii.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gdabmivef.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gykxedpjn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gicekppqj.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gkpbmcnpg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gicxgfibd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gvpcetztv.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gsoygkwvu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gazuzwvzl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gtnbazmer.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gspogydmi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/ggarieveg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gwcepyhwr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gmvotubdz.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gqfchqhzw.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gfppjxniw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gopdkfpcm.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gxedkcjhs.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gnzjkjldg.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gjgmabynm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gxfrmypud.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gfkgjykcq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/giztxrwdc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gyqakvqvp.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/glsjqhanp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gbbswmkzq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gpthedqki.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/ggvkqcpgo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gzgxcscic.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/groxnqxwa.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gyztcgxkk.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gvndgoqqm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gebnkkscc.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gzvxzcyzg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/ggkhxwhjb.sHtML


<!-- 参考信息 -->