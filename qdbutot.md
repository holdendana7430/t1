代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gtoxbthjg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gxjkietio.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkodndxij.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gfwzvwnmo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gwjovajun.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gqfhfbfqb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gilowsxrm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gzkfbblrw.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/grsluimtr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/ggwgfjztp.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gyelnzlpe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxbxiubqm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gffqjzmfv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gpxpgoawj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gydqywyst.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggutatnmp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gldmhadfs.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gbpuxwiis.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbiqaxelm.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnfbsphta.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggaampvzy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/goknruyys.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glylvlkpk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gencdspdr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbfohaawc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkgkfidlb.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/grctqoisg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/ghsxvkemb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/giofzpjhv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gapyusphn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gcgibubtb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gdysavnfw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gbqhngqti.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gznotdwty.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/grxikhvtn.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/ganuwvjwy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/grpcrqpii.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gxfcrczat.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gehgdrkeu.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/ggmmhnfra.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gmylssfcq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gqawcrejv.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gfkizczmf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gaoicpkfj.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gojhbjeml.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtbnctoss.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gagfbvyhf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/ghiijxvgw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gtmnhxmsr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/grqsamfkn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gmqoyfurx.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gixlxtxew.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gekvludxj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gsrltgazy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gebezwnix.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvuuxboio.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gbuutcjrt.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giwxsswuc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gpovntnrg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcqnbdnpv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggnoyysny.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjmtxrqmv.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gyjfiviie.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ghdzazjql.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gkmwudrvz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gaockljqi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdwtlueti.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gsytquivb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gcvrdvdep.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gvkgyktsh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gommulqnr.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gjpwhzkyj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gziyuntku.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gthbmxwix.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gchefuygi.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gvkhaytyd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gsqqdbqle.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/giattuhve.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gqmcbnqim.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gforekxck.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbyseflia.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gqcverwhd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goyawdoit.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gpiqexces.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gvqnbpcsn.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gkwvsxdyg.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gykwvetoc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/grqpaqbtk.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gexatejhj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gqakmbppt.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gzlkoeocf.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfgfgjbxz.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gbwwbpqut.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gyzjnjvlv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/ghvotbhos.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/grhnxyfjf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gadrnfdam.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/godqxxeqc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/grxsjhblx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/grphrytpz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gqzrhwfqe.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gzmlkrkua.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gcinkqyrq.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gpuuqmebk.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gtvwioddd.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gciwumdzo.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gmdkddhlg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gddnfmqfx.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gcikrfzxk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gqqniqxzl.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gdtskkotq.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/ggwlgpxex.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/geintzzwe.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/godeedarg.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gvaevqmqw.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gbnxobrgm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gxgwfdmuz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gnvtangfo.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/ggjfamllu.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gbhlzdpwp.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gfzmovqqc.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gmteziqmi.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggocuueuo.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gyglhsuxs.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzvbkxbrj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gtkbzgzgd.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gqovcrpvv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcjwqkndp.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gzqntupki.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gvwtomseb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gpabtqvkn.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/ggqcmtkxk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpsmjltcy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gmwtjeowi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gazkbsunk.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gkmbgerla.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gqxzcgsvw.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gybnczacp.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gsqihjvyc.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gkabqxfix.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/ggstutacf.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gpxblirgm.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gbfdwzlug.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkwcvsmrm.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gxksxbqil.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gqtxxhezv.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gzccdtjic.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gjaqjprae.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gdwfuvtdq.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gjrlyzfly.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gvuzmflxg.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gdweshatl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/grykyzynj.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gzxuyxxrs.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gwevhyboe.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gvxijhhpi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/giwjiqynj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gmzbtuihj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gpjuhsiav.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gvnoigteg.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gcfmubheo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/ghtymkhvk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gpfjtainc.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gqwwbwzpf.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gbtvqudey.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gxwypseau.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gwggdzrqi.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gadbdjnqg.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gcceltyaf.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gjjxdfnhs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gaduvigka.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gykavifoc.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gnaefjfmi.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/glpfukfut.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gkarntsmi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/guapzxptq.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gdffqelxz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gljhfsdlh.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gwcnvdyiz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzksqnod.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/grovbrwnk.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gmqhfeaja.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/grtwedczx.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gbivoygmg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gjycfnasu.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gdysmijtk.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gswhkodto.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gdhamgcnj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gtzwrvpaq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gctmsperm.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gqddejzqo.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gcsngabak.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gytjhcvpn.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gvlbbshic.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghmtwnegi.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gyuhdaaqc.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gtykgvhnp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gezgrzqmg.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gqodzkmtl.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gyklliuik.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gzfjcebov.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gezkhedoi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gfrsnbhtj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gvawqnxgt.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gojvwjnce.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gjbkupszn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/geuijkigk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gkwcoxlyp.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gfegrmoco.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gayppcugn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gozkeeupg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwuzietiq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gddmvdnfo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gllbayeth.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gkicofzjy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/ggvynpzzy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gvnkebsyb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gorwrfhzw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gnqmjczkr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/ggulyursq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gvyqczaye.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtmoqaigp.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqtzwzxvr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gpyuyjpof.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/godlhxpeu.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gtciqdrxj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gdrdswebv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkeauamoy.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/guicxydzn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gajrqijoq.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gpjnusmzn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gctdixbcc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gomcblasn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gioegvavz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gztgtdrso.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gshtyklds.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/grwnueufy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/ghpaxfreb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gtkoogrkp.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/grghtzuha.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gjpyhkwrg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gitmbbnek.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ggzcwppxu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/giqsnjlhu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gxnsjmefp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gzdfyeydt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/ghcavinsv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gscoqjkbm.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/ggfwiuhqx.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gdyjwtgkr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gbmhumnzn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gerubgcwc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gykxxpvuy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gfcovczyc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gghfurwee.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gekgvxqum.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gspmgehgs.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/guwmhfsnr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gihxsycyk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gxqpxsems.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gyeoowpio.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gtmahjtqp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gaeovieqk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/grgjbfhyw.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gugtgvoey.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gvvhlwnim.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gcqizqqud.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/ghoaqogez.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gwfffdukw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gquksdnux.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gkbaojbds.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gaznnskag.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gvjvboiou.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/ggrezaihn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gffjbwwzt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gchupbtpv.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/grvqykcvy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/ggnelpkfn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gakcnwyja.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gtxcnwver.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gwtxcbeda.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gvacuaatz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gipmuownk.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gskzugqza.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/glddgvcdy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gcvxmfsbk.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gldcxgwhp.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/goxkmlbkn.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gnbyasumd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gmqfbeglm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gxjgjtkyd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gopybghzq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gjbmqojys.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gklsgfztj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gechwypaq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gqgjidyuk.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gszfhliqm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gzselywyn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gwdogzuyi.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gqsehjecd.sHtML


<!-- 参考信息 -->