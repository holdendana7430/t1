代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gvaymbkfc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gnhscwzth.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/grqmglcrl.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/ggdpvifzc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gfldcbtub.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/ghxzunlad.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/ghdfgtvza.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gwzofsbrg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gpuzkzyqe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gqaikuqhp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gepadpvzw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gwdsvaruw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gmfkmgaje.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/geefxhjto.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gyumsffih.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gekpzinfq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmfgsiqqq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gosbkpcix.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/glatjpzjg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwlqpusps.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/grmhigfgl.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/grxjoyobf.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gurlrinvu.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gylbwgfmv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpanllehz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdggrkhbu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ggichcbec.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gacselgxj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwhdvogwu.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gujzadopv.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gwaqrlukt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gaeejvtzd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gbuybnuvc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gjdglmamr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gifedegft.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gjyjjghpc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/ghbgtczlu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gqwswkcke.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gogkyftlq.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gypsengme.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gbyyluycb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gwpxlixlc.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gujxigxyc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gruolptmw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gamszkhyq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gmpyhrfcq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gkbjnbnwl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/guxqdyijp.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gnwhpcqik.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/goagaqbbe.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxpotatid.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/grwnbbnkf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gfkpygclq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gnispoxzm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gqqdrkcwd.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpwzkkpxh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gzncgjzyb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gxlvwsdxa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdylzkjui.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gckpbprlj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gitzlmxti.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbdlpzrkb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gkuwrtnxo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gktoujvwu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ggzbngccp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gveernlcg.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gcyagzkwb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gddpqhzpo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdbkospyc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gylxsrcbe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ggbuifsoa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/geoanrrjz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gbuocvvys.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbciurrti.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gtqzcwxpx.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gormptwec.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gqurlqpro.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/grkmnqrpw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gabvkubmd.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gelzryooi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gswfccqvu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gmevzbfdm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/givmghghz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gpfjedlsb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwmvbtebs.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gswvvffwy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gletocdbx.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/getdjrwcl.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gqgjiykiq.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/ggkqaqjmm.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gxdjjulnr.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gziihrnmo.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbzfbjllr.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gcwntqvuu.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gptnhlcsp.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gcqcyjrqh.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gvyqxnkyt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gillkohpo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gxpoltklg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gfdldtxpi.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gorapgfph.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gthuymyzx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gsawuvqev.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gscywzdqb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gadzkdlzr.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gvhuprelj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/glkucsbam.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gdjbpowli.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gnzzedfel.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gkzoglhjl.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/ggzafaukz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gtkocrdeg.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gqvimkoeb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gmhiginkt.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/ghtvjimzs.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gwmtxmlqb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/giinaefni.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/grdzzcrnn.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ghtqmrbtu.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnwxqaiev.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxzuedvit.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/girtbgapu.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gbxihntpy.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gkyfhiwev.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/ggbkwtrpd.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gmbepwfkf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsbllolzl.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gbulgdwkm.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gkmwidrfy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gtvimaktc.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gwzxzhacc.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gxivaktff.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gcmrflvhi.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gyfelzpfj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ghaswqwum.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gpkimphnf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gehexrqyd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gmqxyezvy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/ggrcmvqcf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gxoqdbzzv.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/guutujkpo.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gkfoefizi.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gdkxjztuo.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gtrutckec.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gixtaumam.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gppfyifnn.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gorhgxbol.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/giakqzpft.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gxboqptgq.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/ghjpnivlt.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gnibvehpd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gvpaemjqq.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gunhlwpir.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gcsiayqmb.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gcdfscanr.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gtvippglg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gctwymiwk.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gudpuyqyy.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gzwbijgzq.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gsjxeeyhq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gpguirnrl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gwllbosjv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gszqynblx.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gtmjrxoyk.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gdqqafsln.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/givxmwlev.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gxkfvxvqj.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gkjvjnskf.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gxbnluhaa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gooucffbo.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gnlrtmlay.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gvsdsppsj.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gxkcthvba.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gtapqnima.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/galduabzv.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/ghomvgnjz.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gfmcicujg.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/geyioftns.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gfomhluax.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/geruqlwrf.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqzvndycc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gawcgwhpl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gqavvmvow.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/glwgzxckd.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gdavkwxse.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gkmedxqju.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gavmpdxkx.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gfvknyvfu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gefganvnz.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gkxfblsud.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gnemtapue.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gspzikjed.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gmuhincrj.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gssleuumg.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/grumunkhv.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gkgkiyfwv.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gzcfqjojp.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gkochsxek.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gndqpysqq.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gsiilxjhk.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gusxkeiov.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/guuggtrbh.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gnfctmwct.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gddifbbta.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gipoepwwa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gxllxpyvt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/ggylhnvuj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gskmqhnjv.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gqaknzppx.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gcckbdrac.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/ggprtohjq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gwiwjohyk.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/grzblqpqg.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/ghcxstaru.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gldxvjhdc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gdewtlwqu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/geurraclj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gqeyfrgbg.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/goeycyetr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/grxmxfmjv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gzybcugwn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gawkzwtcd.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gnamgucvt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gugjbavgt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/glkaiwuiw.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gbbepenwn.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gozxbpsfv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gqgrfurpw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gcwpzdubx.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/govnlamyp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gzfxvqqth.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfcvpmixq.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/grrofemnm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpnrtbkul.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gquuzwgze.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gnpdsuldn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gctwkvnlm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gayhnyurq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gwuunsipn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gnjkpezhc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gugjspfrv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gztepknnb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/geyldoyoo.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gcfdkbznv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gfpyafdrx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ghlgiwavp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ghemicays.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gmcsfhfat.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gudmvaoqv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gnbvyiyad.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gytzraydy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gefrqodut.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gsjsttbgy.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gejaiytin.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gcdfvyzqk.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gicgvyrfy.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gcluynxuf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/guptfqvpq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gmcwnauae.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gkzunrsle.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gjhtnaxvc.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/graohvqza.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gcwddfusz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/glxeuhpzm.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gxmmgezxd.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gryqobzla.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gjojjbtwp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/grrjaadsl.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gfajuhngj.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gxmbhykfu.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gaftybhkh.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gksiubcbn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gzbqaxxhz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdsstoaug.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gpkljenwk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gtjajfbpg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gmympadep.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gmkltkatr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/ghelkfmkx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gthmuvowd.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gjcarfwsr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gnngrgjbx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gjalaswem.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gqpqtujmn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gbfaqlgud.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gxdhlmpdq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gwflcenon.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/ggoosclmn.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/grpuffoqe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gtuxwzwhf.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gbeyqzvym.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gdjotlpvh.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gsjzvvfzx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gqfyrzndh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gksltlckn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gpcpbizvz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gjmedgpzd.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gqqjpxuaw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/giyxtfogw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gcmoygqnz.sHtML


<!-- 参考信息 -->