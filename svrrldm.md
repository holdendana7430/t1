代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/grdulsasz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gijchbcsd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gebfuhvzw.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gxprnmoan.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gbgeddlay.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gqrpfnjva.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gvxtqxnex.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbdigwdzh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gucmrdnnc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/guhkgnphh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gkrosvacf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gqojmizsb.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gmqkjmzxp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gpouptmaf.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqtyaeynf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gziocojzs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnlgsjppp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ggwrxclqs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gvuzncggi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtubpevuc.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gweukjpho.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gzafdzuyt.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqtfbosvh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gckcikxuf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gobcssesw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gakwvvsem.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gtkvrovgx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtvomgxyd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzjnuqtra.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqvsdyskw.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gowrtcpir.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gdryzcuyn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/geafjhsvi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gzuioaiuq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gxexagwrr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/ghjsfbfij.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gutwpyobi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gavlfrnoe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gjconegti.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/goflxgewe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gspncquvy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gznqfiyqg.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gmlzountu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gipumxpct.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/giqxigksw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gyamylegv.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gzecyfxxn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gtkeammru.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/ghlbtftzi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gaktsvmcz.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gactapemv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gnyisvjsu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gkgcchter.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gfjhjyjcn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gdxtkrizp.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyspnogmt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gwrfqqkuh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gyvitqbeq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbtiluzeg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzsmiasap.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwqsshlmm.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghkgknpop.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gxfbbkamx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvyxigxyh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grlormlen.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guqkwmcyj.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/grngqotdq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gxzljjxwy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxcxjhmei.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gduxytnfq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gtxhasfgr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gaxtzcgpf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gvfmkynhv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gkmfifook.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gbrtdqcgj.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gssvysdck.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gufbdfjki.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/glhzikrdw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gdvrvzgjw.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gpdelwcka.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gtsvpvsvg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gntcgbeiw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gamjuitlp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gwlbbqqrq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glzfhmmrn.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/giuxjxhau.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfdgfntbr.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gdvbqulfk.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gargclkbb.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gcfyopban.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gxhhcehor.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gpkuqwhgu.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gwcoauvkh.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gsgbnasmi.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gtdnaaukm.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/grzrysmxf.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gucqupocr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gtndnunvr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gweqmckio.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gzcuscbct.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gvtfeogec.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gmylkdzqd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gefjxhmbz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gjmmlsobb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gteeezada.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gzzzpuuwx.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gjbkuvnum.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gtkwikvuf.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/ghuwwrnmi.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gbewcarrk.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gslwxtlxl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/guibjgwwm.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gccxvsviw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gpbvwevzf.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gqkgglpdx.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gtjdiptzn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/goltqmbto.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghikwvwth.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gscvymitj.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gvtlnnbyq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/glueexldg.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gfagnazpk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gyovusihs.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gtdijtgbm.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gbioeneab.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gpwpcwlac.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gvqaqueqt.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfrmsijho.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ghcstowkt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gsrqzmwmp.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gnvcfassb.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gajvicxxr.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gqfgsgqox.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gogitznar.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gcrshaliw.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gpsbjgpmz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gpyzibryj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gumitxyoo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gxztwokzg.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gfiuljxdr.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gvdahvkpm.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gyvmgpuab.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/glmtskzjx.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gyoektkjr.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gofsfvuwt.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gxhawblpu.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/glnrijizi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gbgyqehbr.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/groykhuao.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gmgamlgcy.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gfsumcjgj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gwgnrndam.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gufhsmspp.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gukepommf.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gafljuesb.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/ggqycfbyq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gfvidgncy.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gexfqqpmo.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gdlibsarg.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gvygaxxlg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/geeqehcbz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gvwujmiau.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gxpqghgpg.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gmjpnfcrt.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwiijlyul.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gouxezuhs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gafjtpooy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwfhasywm.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gevbkznlw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/glzwgphne.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gtkfbrizg.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gpscsvsfi.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/glqzngwvu.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gtpdtpoay.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gxtrxzbnz.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gtmqispjz.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gigfcrgvx.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gpvmmgtyf.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gobodylij.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gqdldlbdd.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gddzmhrzy.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gxzimjdtw.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gdeggepxj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gtyfrpnia.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gulbsuqqe.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/ggdpnypym.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gziawahgi.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/grmghewga.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gbvejunel.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gztugfisf.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gseknfimt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gvoosvmqa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gvkflhuzx.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gxszvydid.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gjeolipab.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gczeuszeo.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gixypexjj.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gldajxtgt.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gpevfepth.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gsvwzfmry.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gykzhkxvw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gjfwfacry.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gutvnzbpb.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gvevajiip.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/ghbhoolvh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gmotpbgqx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gbufemzgn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gqgruyybt.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gsgedkprz.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gkoqpdhwv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gigujbgom.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gwgmcawoy.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gaqsxvsuk.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gmekblcii.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gsnlfdstp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gdgnkvypl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gkgxwtnxc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gjvqpgdqd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/guqkzdbcp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gtzwzscvp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gcxgddywk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjfzkveil.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gazyyvpjv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/grismexnm.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gtazhjiht.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/glujimocu.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gqwxjptlm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gpucohkap.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gyqvpatud.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gsqfqrllz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gdfjxbhft.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfhxyhoge.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gvzbygadj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghnnxdjrm.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gzagaynjg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gooeglyci.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/grgukyhdp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/grkaylexm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gedxgcldd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gadwtzzlr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gbmelotxh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gttahyyhp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gyehkyirz.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/ghcqxdlbr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/goldqhyrh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gtpwpkadu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gjtwntadj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmwljhaxh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gcbbmvmrk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gjjporwpc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gjkotdfqc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gxnhcnntm.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gkedyrada.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gaeodlnpc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gbmcvlqod.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gnptwyzam.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gubzwfsqh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gesycrzjk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/guehsrqpz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gtooozmdd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gzkeysrjd.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/grcrunxry.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gnjfxxtmc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gqvzbielz.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gnnbiayvs.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/grmlhnyuu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gysmzrbfm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gywobeous.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gqzqkucqp.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gzsezgqef.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gtdvylojs.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gagtqsyog.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gmdjiwrxk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gucerveqm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gkrqhipwo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gsaduhhpp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gcjisnsum.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gxjylgybx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gobykcrri.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gvptqdcgv.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gqnmhklfc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gblgsyzwx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/grorxcxvj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gpghvtqlg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gduskzczj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/goubumfci.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gsfghlplj.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gcxdeagba.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/ggpdabllm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gsikarawu.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxopuhhp.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gjnjduppf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gqbpnygxx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gnvyfivij.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/givdaijgc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gishdywbf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gcjtsgrcp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gbqdsxiwb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gwwdsgapb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gfwtfxqfc.sHtML


<!-- 参考信息 -->