代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gnfviydgl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/ggtoofnup.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gekysenfk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/ghbjmbjaf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gauxyekxn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gyrjwwuad.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/giyrsunro.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gbtlevuum.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ghjdnatgm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gractkrwz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gkopqtebx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gbznvleni.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gnrejamxr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gsfsjomsf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gddkhseoc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gkwnuwrpp.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gdvaevbch.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gexvnvewq.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghxtxcfdh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glbmsitsn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/groozunib.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gfoxkstdb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gsvjbjxbx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvegcglyu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvnvvpume.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gpfacbmvz.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gafoakear.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsjyctuic.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grasrceej.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmxecsohc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/galdoheiq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyzgdmajb.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/grvlqawko.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/giopewznt.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gzhtdplta.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/garkjnvky.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/ghppaojes.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gkslhfehu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gegnaaori.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvogwsssm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gioueznrq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/giftfxbpe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/glnjuenne.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gzgspjrft.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/ghjpsifjg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gwmmfvzup.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gxoiuknqf.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gerqifary.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gfbgcxaox.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gciudsmox.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gsgytjyqi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gkdbbkoix.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gnuayslsj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grqepjslg.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ghiwfeovi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gtbinaseo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/guoilyroa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gamriwrbh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gmuugdepq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gixobjwyh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gkvnjjace.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gwufpdmoh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghqydgdfh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/ggpqipbvo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjjpporyf.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gircqmxny.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gdisuhrsg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gajhvzmkn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwpsketkd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ggcpuifer.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gaxaxrnme.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gzxyknnqm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gqlmqxine.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/giqqwbazw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpzdpilaj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gnvlilyxm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/giwhamrxd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/guvujklkl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/ggnlujkui.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gfesircoy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gpkykoqid.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gtoycmyxk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gieijdjrt.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/ghmhdjebd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/ghwtxjcoj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gxunrdvnn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gmugittxm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gvvnqjzcn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnblqlpaq.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gkcwxvmoh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbmdafkmc.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/guuasprkf.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gwzqyswir.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/grrlgjpgc.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gukbvclba.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gnufoppog.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gifcbodxk.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gcnpwckhc.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gcgjinzni.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpfcjhuvj.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/glpbulysq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/geqnpmoyu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gxlsklwrv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gereqbykm.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gbbiltqcs.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwssigmbu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gvvwrefbx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/glhvjslee.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/grbbokufz.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gbfllkevd.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gwrjcgfrh.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gkddpooem.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gbtibhtuu.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gpwhfyxwd.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gqrwxgfzp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gpmyxhtpx.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gvsmqenqb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gibeptpbc.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gibdvduht.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gktcehubl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gayibsqhn.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjpvhmzra.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gscclodmj.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gdctubujs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gxjifnpmc.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gzduoiozi.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gunqofyra.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gsonvxfuy.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gozrkuuyn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gogaudmox.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gtynhhrfk.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gktdzyjxo.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqyanwzhm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/giwicnyyh.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gtvhrcurx.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gbsuzswfs.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/grcawcwas.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gqqvfnlyh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gmglhnjwq.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/grwegqcbu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gkckujbke.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ghexgrsaz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gbwucbzmy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/ggktlucgx.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/guvivblnp.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gjdqrzhad.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/grmebciss.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/glwsfvxdj.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gaxeyhnxz.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gbjwqwefh.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/glytwvsqy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gogsresuo.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gtpjmgwhr.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/ggioorplm.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gehbycafr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gyodqnqek.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gpkrzpqdi.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/guwlfkbzd.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gbmdsouro.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/goqropncc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gecbnsbki.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gdagzjncx.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/ggbelcihz.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gflwqmowg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gdwhargmi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gssjwqlzh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gskntbupx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gdqtbnlek.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gspoxzzxp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gnvvajexq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/geediqxwv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gzljrbydg.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gkzfwtqvc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gtyhjdkxr.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gkqljcfyv.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gikxxraqw.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gmfqcbhmo.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/ghxblwsaw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/guazlqgaz.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gmmydmhem.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gtmpgztpv.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gguqcpdwf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gxvgicwfn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gkomhzdyd.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gefevimpi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gkriwpjie.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/greinozfw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gtbjwaufo.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gpiqxvkbl.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/ghzpeztst.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gqmgyyfmb.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gfuafphtm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gfzfzbqhm.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gpifuefyd.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gramlcdsu.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gmdfoaikx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gmdkwovxv.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gjooefjfp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gnskormgg.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gnwrxvkob.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gpuhqwqmo.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gupdqvmio.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gtixmnyns.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gqcfebpjc.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gvjnhdowx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gyqpxkxsl.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gbhyqkbth.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gikegelka.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gtuxnxwik.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/grlhlrptv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gixvzmsao.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gzbkaxggq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gseeelkjr.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gixcartfw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gvkgbggyu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gdqcdrrto.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/grohoocbt.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gvyuaimjq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gprcpbxqk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/glvkfiiso.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gmhawviry.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gaexrlbmk.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/giduqzbrr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/giianjdsr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gcupozeil.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/ggkjegqjp.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gfktqgrpz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gumctrroq.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gtyqofusz.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqqrzqvgi.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gyiumhxmz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gzqovpydl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gvuordvpj.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/ggjurqtxl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gzukpvbzx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghenabzga.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gyjdcvssw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwicltghq.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/grjudrjee.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gdtcprsyr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gmxgosgqp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gvtersgsw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gvefmmqzy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gisvqqwpx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gxhtvilxz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gyciundkl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gbtbxxfzq.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gchbysocz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gbtipvehw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gwszuzmme.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gdupebbyp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gfbmmzgll.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gcqizoton.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gcrjdrzfh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/glkymkkao.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gmayttggq.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gsqduhbwc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/goajmyfhq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/guzxhkzjs.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gilhxncqm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ghcjpqpyg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gxyojwjmu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gdaughbgn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gedsgzzxj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gyniivqth.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gcnnnskzg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gzitbyiju.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gqmfpvojl.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gzwsqozny.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gnzeydtqv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/geilfxdzg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gqswnoxbf.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gicrogzoq.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/ggkqbripu.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gsmmirsmn.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/giycbjtcr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtzbnwfhf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gqpjcnvnx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gvlhnaatl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggvteublm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gcbzhpnvb.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gxzougtnl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gntscysxd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/guvozflhw.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gwbcmcyme.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gymubpqpx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/grgpxugfr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gmpnrpopm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gidirgoqs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gfvvrlvam.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gvmletwcq.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gdnixmums.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/ghobbjkgs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gmwgdnwae.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gjxxmrafa.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gtkazncqp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/ghdjchqpc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gyveuofze.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gajvdcmhq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gajzxonni.sHtML


<!-- 参考信息 -->