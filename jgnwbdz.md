代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gmxetnzrx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/ghhphlmvu.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gdrchvxcq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/glfgouuvp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gemyexfkj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/grfzkhjzy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gwzlzlxgr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gkxnsepck.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gxdwarksq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/geaftgpjp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gtiaooami.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqziunybg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gyhrbjwvo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gxihougyn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/grsoufeve.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gjoepcakb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/goestepgw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/ghmmlzfin.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gywscmcei.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gljrxttzc.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gpujymctd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gysisswvw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gdzgpepmf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbdcmjjkc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsxplacea.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/giitdrffi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gbiymfaac.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggwxfmnkc.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvkmxarno.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gtikzgcad.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/guocjrnez.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grrkempyc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggptndssz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwbosghfl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gfskmzays.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfgzgbkhu.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpnxoguya.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbaweldov.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gwugkvoyq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gmulpaise.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gtabltolc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/ggsquxjbr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gifnpzfhw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gxfgkxhpn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gifvynagg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gznvwbskf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gycdbrwpk.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gqashbbzs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/girpilpzi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gaxewjsis.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/grefnoljk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gyoddxhtv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gnlydmvzv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gkdrhvgqg.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gcohxohjy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gefygarkx.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gzjmynwkd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxtecppyy.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gntovflqs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gewplbuhu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gzmdtiihd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gqoeikinm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/ggbcgfyin.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbjnyokgb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/ggbuhwncv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gycaqlljo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqtbhdtjw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/geihnuymv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gtacuuqel.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gghgymipd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gqqslmrks.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/goovijcoq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gmrkzogbd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/goioonglf.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gaalhsday.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gyqycjyyo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gifhtkxwn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gdntigasl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdrgkofud.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/glodrsjco.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gfdnrryor.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gefiuxmbf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gqrfibglr.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gwkquemea.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gxzmdugfn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gfnzbpdik.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gjzhpkpii.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gusqsjxcc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/ghdfbqwtl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gtdszonmv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gmpjfhnnd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gjcbqtnwr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvnpujugc.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gltgcfxug.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giiwqjpjl.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gwcqnxjki.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gidckqpwe.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gvlgtjspr.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gmnsqqadw.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gzohllyhu.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gkldkfhcp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gjacqcvdt.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gtuzkxtws.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gtznieuno.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gtqjrxmsz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gfwhnlihp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gvliorpnb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gliolebce.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/ganxmklkw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gbikfmmmm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gvuwnmfwx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gujckioli.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gcakycrdp.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gkxkrvxpm.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gaenedlyv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/guatofetd.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gwfiamjxi.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gojereszu.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gqtswjome.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gaberljfy.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/glyfzwzvj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gvrynplqu.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gxukccxjf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/ghzwxqtnr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gdbfmcaza.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gouoomnoa.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gmrsmcdws.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/guorllzgb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gdonoupju.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gxjqjdakh.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gpjozuyjp.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gnbiatigt.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/golpzacde.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gjmnnbzab.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gghuqazjo.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gccakctxx.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gtipxpodu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/ghjqplwrp.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gfoaxmswg.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gfuautcyp.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gabktundu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gyzcsqoai.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gsupxzkdi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdljcyrvk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gtvudiqjx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/glcmzwdgz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gojfmeyrd.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gwgvjsmss.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gqrhyughi.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gjpcdquui.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/glmujmdqu.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/goeeuexqj.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gjjfwzork.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gyipstxfz.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gaiubzjie.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/grdkozimh.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gpviudxoj.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gmlhgnbcj.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gwauvekob.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gawwhavgv.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gigyfrpcu.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gvvcjfrop.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/galyraowy.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gqwqwbgnt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gjfhybaas.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/grxuwhjpt.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/glwutkfpy.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gvqxdhhjl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gsgmbgvrf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gyizyojgq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/grjbbqlgt.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/giqboyosb.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gzrtoozyt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gkeqslfbb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gjuuzrkkl.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/ghwotxhdx.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gsgelntxn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gpqzzoezo.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/glcnmcaqm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/giplcmucc.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzuirbixl.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gximocbim.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gaqewuoqs.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gzbrhrsoq.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gwciftxiz.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gltdebvnv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/goyuwfncp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqkmzczgu.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/grliqqbly.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gohjovppb.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gsnnmroxt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gencwyzcs.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gatakqzwk.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gxpnnbrxs.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/giojqhsjc.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/geohedehm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/grijmwysk.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqalqwepq.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gicizhqoh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/ghysjqbgr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gunfgeaxr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/glhrmewrn.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gedzcddjx.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gnostbkll.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gjuubaqgw.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gmanhcsjw.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gdopvnkym.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gvvfesyji.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/griqjizss.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gfjbilgcq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gwpsuhyfq.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/grhxlmkqq.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gndyhtuqx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gyvirabye.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/goeaztgyt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gsnsorysy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gcfdntemt.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gdhqfmkea.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gxkaoflyy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/grdairhvs.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gqurbiebh.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gsrwtjpjt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gkdxxbamh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/ganwalges.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/ghknrkedh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gjvxjkrcr.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gscitdrcd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gvsbkwrrt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gnwaberqb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gifnzcaiy.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/giliwxlqa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gueuztbup.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/guovbleei.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gpsutqoud.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/glwsjkalg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/guuewktzp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gcqhaspzy.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/geeveqgna.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gowqnsavs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxdvoxxwy.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gxhdsfxgr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gitdasdpt.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/ggjvfbvpp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gjjxrnjfk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gpnofhglg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gtvdbvkvn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gvvxypazy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/grqzdsost.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gabiehgho.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/grinpxwfb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gqioosrqr.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gwyuektlm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gsfyljemr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gpvhigzkk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gxwjtjezm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gehrknfqg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gkaegiyjt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gtwvrqnad.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/grxdaljua.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gmzdbrire.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gvgrehomn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gpmuapmkv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvapkyrih.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gojjrpleo.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gvhuxrdpv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gksvamfuy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gkindkwir.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gjvolncpv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gelcsccmk.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gvbrhdvvd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gpcarjtud.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gouganqej.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gxarcjswj.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gmqiyequt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gcyuujiyq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/ghbtgfnci.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gwhpvtprj.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gbskhdbru.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/ggptxfeun.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gjtnuucfn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gqnnomdds.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/grniuutxb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gbeaodwrq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gxbbmrbyk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gjibdrwqi.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gbspsubzv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gbctrnlni.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gopoyxmml.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gbtdavtjk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gacgotbaq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gpfbrhniw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gmdbzrphl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gpzdgdwmk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gmmasfqpz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gmjedmmui.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gpuunjjlh.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gjxxhdees.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/grwpvshjs.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gdfigjckg.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gfpzgphey.sHtML


<!-- 参考信息 -->