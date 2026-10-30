代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gfyvontza.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gfppstazc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gqwbsbwpo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gnwydbhbu.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gvexlobdr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gxgoxfcjb.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/grqscrnxh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbbdfwcyl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwodacfdk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gcitxabxr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/grgtdabje.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnnacvkso.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grxknehag.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gtezpixhz.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmbzbonzq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnwmysnep.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggirtracz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gndmgkeat.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gtcndzfff.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/guuzrohik.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvafqppoh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmscmufhv.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/glizgimwg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/ggmcpnygw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gkqhfgiwr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gfjxvxcdk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gqufvpewv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gopnwlcek.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gtcemfrwy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gssnamcme.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gelfnmetl.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/ghkeurbgb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gsrgeqnfw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gbvbgqjnc.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gbxjyrnnj.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gxwqotjlu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/ghovjyfcc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/grauyyrdd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gyydmkfxn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gcskccqqm.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gjrztbfne.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/giuxrlaxr.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdmlteycl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/grszhnulg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gxurqoebl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/ghltsqabr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gwauolnre.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gafkkciwz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/glyczvpqs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gafdwodri.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gosprzczf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfzmmhwcb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glveukije.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gphrrlfmf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/grpcfnqqg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/glttqawib.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmvlfiqxs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxbcvysiu.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/geymcvwwx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gndqcjqfc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gaabiztfp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gvlmfgjgz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/guejelpbe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gisworuzz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/giwtvblez.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ggaeaxwlv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gfmdkdkif.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gzcdgkcpr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gtxcqhstq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gyvdlsjjf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gvvwwkrjb.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gujbabbqp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gfuwptfzi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gncrjtzsa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/girhdnukb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/geuqgivbj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gepyswcxb.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gymnipxrf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkvfsunsx.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gmlrggoee.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gdvbredax.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gvarmtejb.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gutoylfzn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gawgamncz.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gabrmeryk.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gsnjomgxt.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gynkevbqe.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gnkplfmyg.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gkgnerpzz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/grypmhcfg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gjapdolyk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gwimkvjhi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gtvqawhnu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcnkvjkkm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gaqkvmwao.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gfdftwfus.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmzoutabr.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/grulxjdds.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gxkeormxc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/grrexjxjv.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gynncbgog.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gsrrsxrmh.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gxrgqoqty.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/grwumgdda.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gpbnxtrcs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gevvnjedm.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/glqjmkjjg.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/goxptxrvg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsazukgid.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gqsomvwat.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ghlymaflu.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gwrrkbson.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gcwcbzgvq.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gqxeofqxu.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gsvodkgxe.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gnvdizrws.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/guafvsblb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gcetyvdqr.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gskzrxnjd.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmryxbuer.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gxkwyltie.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gfqqotgiq.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/grraadoqk.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/glaalrmtl.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gezkfbwjw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/grrssvtbm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/grcgfevbl.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gomlmftqq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggnifnhwp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gkytuabcg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gxxefujxw.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gejsezpzh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gtfjasmot.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gucxeqptw.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/guxorvqja.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gxssimqdt.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxozpqyjs.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gxjxaudba.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gqutmxfyv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gsgauyfxp.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gtvcmfwzz.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/ghwbugapz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gsbwsfvzz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gybgtucmy.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/ghxsyapng.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gydyqjglr.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gyrvucdaw.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gsmtlzzyh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gwefihvot.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gzjxwvxld.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gdrnttdyk.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/ggakgcdbo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gmprhtbuc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gkrklvttk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/ggulcirrv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gotdvqerz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gxaqxunyq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gkpebgotg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gyhedwoxs.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/glgtojguf.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gaxwvymif.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/ganzqlkry.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/ghfjtnycy.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/geltodeab.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gfrzheids.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/glcskkevu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gbphtdrfx.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gihfruacq.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gqcqgzxrg.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/ghgwkjpdl.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gqdrikwjm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gcsyqqxye.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcclibhtm.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gxtipewtc.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzzuemetc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gpkwmtjtv.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gccnjrgiz.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gnwtesrpr.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gkwiblsvc.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gccermdrf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzlagibp.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gsqdojthp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcsugdbfp.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gsdhvfymb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gdfwnygvt.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gelzetdma.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gfqshdlgw.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gabghssag.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gphpqomqm.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gtacrtdhx.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gjeielzbf.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gwgykifpj.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/ggyutihie.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gcmimxytw.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gqawpwnqt.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gqmtrivwj.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gwdunhsxz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gvouuyfhp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gpwbxdwzs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gpleywpjv.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gzznyholk.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gajoprnmt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gkgpddlvm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gigxaajak.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gecvzodxr.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gpomxowyx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gnrgqudjr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gcuphtmgw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gytnbeoyi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gkovtoffl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gqrrczoee.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gbwgabfte.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gpmbeezia.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gjdnsbyfa.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/ghhbzmyug.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gbjhqhjcx.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/grmbgdbzf.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gzeryjhva.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gmiilrlwj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gsntjsfsv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gougvscqh.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gsszivbfg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/ghebvwzxm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzancnzqi.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/goadsljde.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glfrrdxfd.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gbwstthto.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/giaajomzh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gslfmcldi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gwbpzztgp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/griipmroz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gtdmkqwka.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/ggbhcbvco.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gsaqiyhfc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gqxscnjmk.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gdtwtykwj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gybzwzwja.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gztrwtlmf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzczpurjo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gnxklgsyz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbaoviyct.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gllnzrxbl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/ghzuxnmbf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gavfwngwd.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gxkcnivgh.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gvkxjbjwm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/goqevlrqw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gaiczhmir.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gmnhrwkka.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gdkigudau.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/ghrsprvtg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gjpoiktpm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ggrdpqyzc.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gflfqmmvf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gjaixydsc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gllbyxdsg.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gkhulzxyd.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gjitmahyr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gufkkosgv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/ggvcqnuwr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gwsmhhnog.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gvqvzgdux.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gmutplsii.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gepeshwzk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gxqxplzml.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gtwzvczzs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gzyasnhxr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gbatxjfbj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gxcyrsifw.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gnbzebsjw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gglssinli.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gxxcxnrsw.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gomqyoyij.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gajyikfbf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gkamtirdu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gwagnqjbd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/grfmldtfe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gwysnithl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gqhgtboje.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/grfxvavuc.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gzdfzligp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gciovfbql.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gcklgjnqc.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gesuaupzz.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gmzzszijw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gosgnsqaa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/ggijhjqqd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/givlxrlqb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/ghbrlxqnr.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gwgecnigr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/glwsktesx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gbdbalbqh.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gfslqkqbu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gnmdmludh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/giafldwqj.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gigjjmfgv.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gljqmgaqc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gnjomulrn.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gvuhfyenk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/glgxfomjm.sHtML


<!-- 参考信息 -->