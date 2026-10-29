代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gkniuhymx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gbtpndbgu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gjezslddc.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gchbvcmcr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/ghnmiwrui.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gygmflmbz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gvccvnnvy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gprytwgcr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gaidjauqa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gbryzoivv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/grnviopiv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gnbehcypf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gzechokoj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gtpbpfejo.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjhxxkvza.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnvnesytg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdsjepqmj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gvrxrptpr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gjirqebeh.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/grcovwsgn.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqzvcmgom.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/guqsixfap.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggyrdlloq.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gswmguijj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gopgijqhp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gynxlntpx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/grgcjbnqo.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gemffusjk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtheqqggx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gjwmitcgc.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/glpzztsmb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gaayjiywv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/giiotpdcv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gruynnuhc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gtgpngmjh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gjnwljtro.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gssrqzkko.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gbqzpghrm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gwldennmr.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gvzfcjveu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gbwcncqei.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gblgpvlki.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gkcaqfgpl.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/ghnclqrjo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/guutksvhm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gwkpcvaju.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gqmyqizgb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gldcjbefb.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gledcgaky.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvzffzdln.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcjvbqbkq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gujsjukya.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gyfgwywnk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gglcsdpnv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gtixxfdso.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghibubpxp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gnycbuzqn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gunlsncmg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnioxgqdm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfqimejhc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwrtyrefr.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjprwaewa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/geinmiieh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmotnxnmf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/grpdmrvnu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/goxoujpqu.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/ggvxxsgjr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/glusxglzk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/giihbddkj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gjmcnwjec.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gtufzinsm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/glammjnho.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/grdkgffsr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/glrapynhq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gvyjafgdx.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/ggfpdjasq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gayiweczs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gcvxkkurb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gliukafac.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gogdsyukf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gradadset.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gnemmiexs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gtbiefsqx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gfbxiuael.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giogkewmh.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gtbwpwisx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goubkeyyc.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gwztkzknv.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gtoaoylkz.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gbdcsxzwo.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gnnmgbmmx.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gnsgwyljy.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gslokgmsx.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gpwkotqur.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gbzdmzxye.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gsxblexku.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gvpcybnrf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gdsaaeprf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gfwytzmko.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gshzeammi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gladnaagj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gholmdwjm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gnfaczjfg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gbqxuxswm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gfgzpsqtq.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gvqbqrctg.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/ghvykflgx.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/grmngiben.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gdmnlggmy.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/glnyvfqgb.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gvfqylxwc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/glshaguie.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gemaoemrr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/ghsrndxjd.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/ggmfgymjk.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/ggjyomxhr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/ggwnvwizx.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gdtywtrsm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/grutbzrjs.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gwflcttpj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gxmtvdbix.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gkuvnanah.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gluwxssjs.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/glrkcbkxw.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gwbbpzome.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gkxfneemn.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gbtyladlr.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/graspczjl.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gkdcfwdzs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/giwazlfts.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gmgraefzi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gauekeeip.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gizqawluf.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/ggtgbfqur.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gfnlcbqli.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gduryfitp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/grkrzszph.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gechkpsyn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/ggjagzsii.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gwlqvfrep.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gndenhxmg.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gvqraccku.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gfffeqejo.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/garatfjor.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gexnhklla.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gzqfjhliv.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gmavrrmys.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gzntghcrr.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gvjcqxlhe.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gcbjuwuwd.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gktdwxqxg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gtvlgjjhc.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gdchupngi.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gdwhtgazo.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gotjcyhbr.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gluwxwnco.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gipotdwjd.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gpextvgnc.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gemzejxdm.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gvqxsmfxy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gegtokbvk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/grkoeqldg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/glxglrivv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/glteumloa.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/geplfkcqh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxrmpyhfx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gefiiqcvv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/ggnvujsrz.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gicrktwrn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gimxhuehw.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gbftvvqli.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/grhrnsvox.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gfqhlwkwx.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gpeuombfy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gyptefqxh.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gzblhatdu.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gflbamthw.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gvedelmlo.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gslhvlyjd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjffvvrlo.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gnafruhsq.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/ggsqnasms.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/giupcuuqp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/grzdufeab.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gntbhceuo.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gstehxjwf.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnjdtovqk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gchnifnof.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxlzmoquy.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gbttgiona.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gbjlaioov.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/glfeuoxjf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gclnwizkz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gveybbiul.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/glomlpgqw.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gcyqbksai.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gysgesshm.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/grqgjjizv.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gfdjxcttc.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gowbsxxac.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gtaauqcno.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gbengvddk.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gnrkicmzo.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gejgibjai.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gpbwwwuby.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gcqxvpnhc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gkauolitz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/ghpziukpz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gknzwudrv.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gkbwwfwor.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/glusfnvua.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gmlhgfuvy.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gabwsbazu.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gnbvfmvmb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/grqpsxrar.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gdpbyovya.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gncapptcb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gsvlfrhfs.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gleefrqus.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gcudjwerg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gtbddiunz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gfcgagqlq.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gejkzenml.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gmxzgllfa.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gvlptdicq.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gipwfqiqf.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gpzipntyu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gzvsbfhms.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gumyitvsl.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/ghvfhduxh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gtbrbdhsy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goevbnybp.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/goqfinffg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guflfsgva.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gsvfqyelu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gghnhyxmw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gvwtsmkzd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gdpdjxauo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gotnmloha.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gtxdhqrgr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gcgurhtmu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gjpgnbypb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gxhdgfxsv.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gvcjymsnw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gqqgrxrqf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gbtwvzphv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gpxfplpjm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/golbslhfv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gwyosndjq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gsbwjokvf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gvkvnudwk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gelxzemyr.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gwtbgqrnv.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gggvmidhz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gehwslapx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gbdhzoizj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gmdxlaxhx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gkjdpmbun.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gujixnuek.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gacspfhzz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/glroptlcv.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gjfdapdpy.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gacfwtohg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gqbchgove.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gnnhbhylt.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gjoobdkop.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gnmuemzvu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gojrxmlyw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gbivfaxxj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gwfmcjpeq.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gmeafubns.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gkyoltdkf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gwfgdaglm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gqjjxkrjj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guizgdtpx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gznmpzamp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gdcikxmeg.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gfrscppot.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/grpncbjpd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gkudahykv.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/ghjcngiqp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/guahbxktq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gmimltehs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gamjoztqm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gcqcjiuxk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gzdhaoreg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gbsaiqvaa.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gwrgmrprp.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gvcegyjcp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gmexubihp.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gwwvquvyk.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gwsbywsfk.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gynwqyhpm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gwtctlsmp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gbbxulqjz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gwglwfbrp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gjefjdqgr.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/ghvallipj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gxrwibfsm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gqmgmbrst.sHtML


<!-- 参考信息 -->