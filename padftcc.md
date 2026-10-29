代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gmvezyfpm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gphzdrifi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gtkwnqyiu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gcvflkmej.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/ggfikpuwk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/grhlbirin.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gezyckdqg.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gkcpotita.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gxtuufwyu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/ghmblejem.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjpmtrcof.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gbksxscxh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/goiigxzvx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gglvzjmdy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gthhegzxs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gzxxiutpo.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gbxcixzog.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gcsfhhtgc.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gsfgbricd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvffbplgl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmztncxdw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gvverpzop.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gmcrppawe.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsnucfkfy.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/glhkcnigb.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gqolbyfet.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gylwyphxt.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gomoeaemg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfrdiwujb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfafvsoml.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ghfewztqw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcxeyrvqr.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmetokfbh.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gcregeobb.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gorppjmcg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gglkeghdo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/glmcjsrmv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gapysfamy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gduezsuyo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gmlmllolb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gnybzgcza.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gggqnvlfz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gmunkpcgi.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gegnhotxw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gexyutenq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/glqpdofig.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gcpwcfxwh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gbkqphqbu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gjgyzvbah.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gqrubyoyl.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/grchyyfmk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/grzkclhlc.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gucsvqtve.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmbknreqr.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gunqfgdhf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gsvgwfvcm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/ghctmfffx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gokjluxyf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gzgttixhu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gweeauspx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/grgcnevil.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gcylumwne.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvmndldax.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbtkcutdk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghquslavd.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gllnbxnuj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gldwwvjpj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grtsuohli.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gomtncggs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnzjeblcl.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gmxiciyhj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ghndqpgox.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gueobavgv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gkywssbzx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gliaebmmt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/grwhekthd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gobyxaveo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ghlbbmpwj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/ggucgzfrm.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gzastwjqs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gzuhkwhor.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/grenpavgo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gikhmbagt.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gkdtibhmc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gtzfrtmfm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gmqontcec.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gtxfciamn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/ghwbkcxib.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjzgvdbjv.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gbyumqwsu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcylnzpkz.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gpyrrleps.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/glhjtmdaw.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gfncukplh.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gvcswzsvn.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gujpxbfwg.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gjtgdsjxc.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gthusrogv.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gyvkfnnys.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/ggsmopybk.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gezrlatlm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gjctbpcrx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gjllgspno.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gqkodltoh.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gnsiisnnz.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/guldwqofo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gjgnrehda.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gvwrtgimt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gnfmhjoiy.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gdjrixnym.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gedcjubxo.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxmuqsrbd.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/glayrnvzc.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gsjyrcekg.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gblwgelvp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gwtpkylyf.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gfjrtfmwa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gumxfnpss.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/glkhksveu.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gsrewiazv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/giufhftbz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gikrrdgmk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/giwnuwtbj.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghmvzhsni.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gglzpvmzv.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gwyfudkad.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/ggnoympyr.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gsdacpcgn.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gekcfqdep.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/goqjbuquq.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gweucynpl.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/glsidylwt.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gflascjhw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gxhbshbfh.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gmdqksbty.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gqtufgnxb.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/ggtjoxuay.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gemmecheu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/glfdsnpuy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxwvauvvx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcwdfhvkl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gdhpdmvtk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gcbbpexds.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gqkbnbofk.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gqpduyprt.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gdcugnwvt.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gvmuxhcjy.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gvxigqgex.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/guteegrve.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gyvezajhn.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gjqdhqawi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gffwsiuci.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gfibdajaj.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gafjhuguf.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gxxcpfjzt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gtutjgxfo.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gonmiagvh.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/goecwzvux.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gxyvlemtl.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/graintuln.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gstihqgxg.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gmmfeveep.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/glxelptux.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/glehkkhjt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gkcdredrt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gatzsraov.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gxkzqaqbj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gklelydvl.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyudhredu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gglcpjicd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gbkoiqogm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gybaudbqh.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gmyquecms.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gfypausfv.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gqlqobcyp.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gdupwxoqu.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gokkcnqhl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gfmsznavn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gvjakmjiw.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/glhpvaomp.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gzuhjvrxj.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gvqmibvmq.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gemipunsz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gznqzhpdy.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gywivrkbo.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gpuxgonft.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gbaqpfplh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gzynpsnor.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gctkattro.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gvgvxitgv.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gvjmiwshe.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gempmlfcc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ggvgrnljc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvftqbinl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gejphszjs.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gwmxidsdf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghrjvynwa.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/ghlylirok.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/ghdilqghu.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gyilceryk.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gokkjxphs.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gvickmvbi.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gqrygndhz.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gzvcojzwr.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsunhisdk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gclmlfxvm.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gergzvvla.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gnrbpqfgw.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gkzcqihcb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gnboqwwpp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gvbdawoja.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gszwyvdei.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/glwpltldw.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gvslwvrwy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gusmozikg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/goxyblbei.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gieergxjs.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gsdigbmuj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/geznddhix.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gzsnggrrh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gdziluhcy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfkbbaeg.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gstvpgybx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gfkiwuytp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gmndzbeph.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gajvlgwse.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gqkniveji.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gmdvljagj.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gvvrfxxor.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glgrhgfxg.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gwexmcavm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/govmkecxo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gdpcelctu.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gvnoqaycu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gnbhtipkw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grzwxtetg.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gotfsskei.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdzqvfskd.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gpjlexhow.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gbvxhuehg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gkbmhtoxh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gvosnuaqz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gxshaovja.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gaxttupyd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gptdbzszg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gyylhtehg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gtqnnmfvf.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gimqidwil.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gmildyily.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gghxsoltl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggbwmwjgd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gjjhlzwpv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/grwmugpfp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/geddzhgtb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gegekrrvr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/goueghvgt.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/giqpzqska.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gcsbnmdys.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gahnwspae.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gzexjlnzj.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gwkaleejh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/geijetqle.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gfhtvkivk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gibugnifa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbrltbpne.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gwxyxskzg.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gzrkajcva.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gzadfyhqa.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gouuxijug.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gjofszeqf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gjawapnsl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gtvoxpyhg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gtprinqxy.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gwzmvzygd.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gdrmfhcxf.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gmxtvrzll.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/ghguphpjp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gtgywmbuv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gdslpgswz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gjezniyvj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gzupwguqm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gjjpxkygo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gfoklyqql.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gdrlyxhst.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gkseoodhm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/ggjuknowc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gvkuupequ.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gjizfjsss.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gpcmopirv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gykibgkcg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gsfbyhacz.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gkdlvoxht.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gctcdcbct.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gwbirimhg.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gbbhxejhe.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/grdjjuqbt.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/goosjgfwr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gfkhhgwwh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gzckekqge.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gsimqszpv.sHtML


<!-- 参考信息 -->