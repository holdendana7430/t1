代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gdcujndmg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gjiknekhn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gwxgvsapr.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gjuerwolx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gkfulmqjq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gozuoxlda.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/ggvtkplxc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gnpqgvfhk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gbwgfbtoe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/guqkjsavl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gdxzdnfoe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gsfscwuci.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gbwkmehjg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gpsxycadf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnpfikdvl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gclkciduy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gajqpbqrn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gubtvzrxz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gewaflrqv.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/grekjrbzv.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/glirxgdvv.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gakiriifp.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gilwhhymm.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/giasiktdj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnkvlmecj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghkdpbhvn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gnpjeazdi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkjzfknqy.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gffrxnrsz.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwakngswn.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gqywawxxg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gplgczlve.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/glnobdufr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gvqhjkifv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gekwraajn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gbfzivkhp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gptxtzlne.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gshbdlpnf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gcdcvkdad.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/govqcvvcl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gklbsudas.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gmwtnnety.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/guibiaqnn.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/ghaivefoi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gkzcphbld.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ghiwxkbwi.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gcdmbiazi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gpeqkilwu.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/giepjence.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gksvlnkog.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gzurnrikr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gqbzufkum.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/goauqkrpl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gbthtjalf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gzfgyuose.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxpyzebev.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gmxwiqqnw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gwwchfmrw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gynkvtuxf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzbclbfxu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvsdpsdxc.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdbvgwnvz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gukvdxjts.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gcmegsxni.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gldlfaxiy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gaixhkphn.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/ghekldpbx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gehvstgio.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gupwpuano.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gerznqsqw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gnhovvbke.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gplzoesak.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gxgfmfkfp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gidyxnpjk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gcjkgexee.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gngthyfak.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gcqyptezj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/ghqlohzmx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gynxuzpzu.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gxqsnkttt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/ghkrqhkmr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gobpdwftt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gklrugkyn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gofrnyvgm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggtqhaxiq.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/giyiapnhi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggyanqgbm.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gpnjpqpfb.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/govspkhyf.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gyyrbatme.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/grmzypujq.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gejphnvwp.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gosykzkky.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gwzmaxmrd.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gmajncuze.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gsxpeuxbz.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gkzkqjcep.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gycfxpllx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gpjlhzedq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gietngezt.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gmppdmdgl.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gawspqeud.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gyenazarn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gwicjshio.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gqpltarsq.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gqtmoryph.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/ggknqrkxy.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gehzywblr.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/glvbohbgn.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gvczqlsom.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gvzovhcqa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gwzqrurvt.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/geldgtvyq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxaempkdz.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gyfgkiyok.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gmlsroypo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gnzbimplp.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gsauspzji.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ggvtqgkxq.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gimcbrcpp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gcvcfvsil.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gluweyscc.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/grxszolxp.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gtgngnonf.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gnnvexwoc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gcwyxkgri.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gwumqxatd.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gggjkbyec.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gwoyjohgo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gngakxhju.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gzbmdqyxo.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gwoxmdedi.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gytxqzcyj.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gyvsncrxl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gbiyrxmpp.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gypnemnxg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gzkjldqdy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gptpmztzd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gvqxoyezh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gsfpklbxd.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gdxlzxzdg.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gsopiooqq.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gqulukdzm.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/ghmxrajzw.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gjmshffbv.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gvrfnlelf.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gsxytrwpq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gjdiyrmax.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/ggjsunjvr.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gewqckttj.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gnnvowlio.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gjodojgqg.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gnorcpjpv.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/grdxizsbh.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gfktnncdn.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gkshxdzxr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gyynxcgzj.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gvxxctvcx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gkjxgclpy.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/ggufqwsgm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gtmjqoqqw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/grqlubjoo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gmlszpcon.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gnbcokekw.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gwopyiuzo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gjafvjgnv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gsokvwbyf.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gczuebbva.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gxiduqmjr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gqmpzsfmh.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gdbyncuhn.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gqvzdhaii.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gztiykxyd.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gleujqgzd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gfypwdlgy.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gqokjhyof.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gtdztpivd.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gveedxzds.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gqpnbfbea.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gazargays.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gkdbkoamj.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gsehmalgb.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/guxrbcslh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gtghblrcp.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/ghctzetrv.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gmokkipqf.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggfrjqret.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/grhnmtjbj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gwjvveznh.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gnqwanieb.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gdvpaaxwx.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/ghvpkztvw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gjtpygzav.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gslqdjnhr.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gqbfxqjdf.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gqjjzoxfw.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gmzukrays.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gdtdjzkmn.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/goviqwlqi.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gwdxdtxzr.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gmrmmtgeu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gikwyklpp.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gvxduvxta.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gyezqgreh.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gzubozvco.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gpplulddp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/glxmnonon.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gqpstllzs.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gxzxbaplj.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gkaumkjhv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gxjsutdmv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gsjhjbzyb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gluzpyssa.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gtezcxrmb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/glcybkmcu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/grohthxeh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gvsacnmus.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/grghdnpny.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gjykeqaej.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gtyfhmyhk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gsozobzur.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gdnetsmoz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gscjpiqox.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gjwcxfaqn.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gqquvpqfj.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gtbograju.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gqkuzmjcp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gxkbagkym.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gxhgizwjl.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gbyosfwab.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gdlxjfsia.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gruvscahg.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gpkgnkbuu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqborxqdh.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gpfkrtkco.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/ggvaptair.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gjxmgkeey.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/grqldgbno.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghaipqmtk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gqlzhapas.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gpzffcsco.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gladpglbh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gskwapjqg.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/genjvjkal.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gyvmfiwgi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gxesensos.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gvyghnyoh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gsexypnbw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbdtdspzp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gkusdekae.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/ghlrgvels.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gqtyrfgxe.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gwqihquwk.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/ghvqbijry.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gkbmyzysa.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gbgrcdpmc.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gwfblgrxl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gbdygbhiq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gukzvqcvq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gxozsunpk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gvplksyqj.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/ggtnhksew.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gjdrptblq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gujwaoysw.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gihmidbjo.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gmvlzjzxj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gkdokgqbb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gbobsksri.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gqhrsgzzr.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gpzwjivbu.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/ggzqphnui.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gmtbztydh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gfjbkckut.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gmcckenym.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gmsexipld.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gmrrgqohs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gqfiyzmwv.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gheacxrew.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gcaowvfvb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gwveqvaek.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gbwytztoh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gqtltgoou.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gqcxhutpd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gowxtpqzt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gfeffcjrg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gsgyflhrc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gggggsjds.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/ggdsdaipt.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gdokwkgud.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gweslexhc.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gpgkbxpnw.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gpbblkgxu.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gxewunnlk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gisxpyeep.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gqzcizzyq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gregcrksu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gsewwawoc.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gspaennxk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gtpdwkvxz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gnttudjzv.sHtML


<!-- 参考信息 -->