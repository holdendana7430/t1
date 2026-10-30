代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gfqfnhypa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gnuvsmyzt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/geqtvkdjh.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/geohawtxx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/ggyehxpcy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gjnqnaxai.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gvbntfkie.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gnxpsukvg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gupwyhpow.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gqcvpwykk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gijnfwnek.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gthtvicio.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/golsftvpp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gkdmspqaj.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gwryuustu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwdjhkmxw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gankpthrd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gjcshyhnx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/ggkhrirul.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghymlwtnc.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdruwsynz.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gdelkbusk.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfmmnksit.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfqiwmfhj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkjjanmoe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gndmsawsd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gypwvxgtk.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gatutryyv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqlpydqga.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdsuxbznn.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gpfxnkdfj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gvlchsckw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gladkenoi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/glywzthtc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gxrnztcnc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gjlgpwcew.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/griciqjrm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/ghofbfnqh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gnxigsgev.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gxfwkfyqr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gdnwuwqmm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gmbhlemxk.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gpukbahla.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gtbvckpwc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gtnxsofvs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/ghptohlkb.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gphhfzzyn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/grqctfbhb.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gtkxhelbk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/grkwalgab.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpzerusup.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gmipzsvmu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gikyxutwd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gwckwdmtr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gobzdpeli.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzvooteom.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gympshust.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gaxbbaiev.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyqsqbmkd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gphghsokk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtedjicjm.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqcwxeaxi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gmdtygckg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwxsaettq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvdksrbtr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxrmpukvq.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gxoalkeqg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gjbdrqoyp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gzuzgenyc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gnyuyejxg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gboycesoz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gpxsiebta.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/guuihgasg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gctopxdss.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/greideicm.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gdlqwxdlk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gmnhuamws.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/griwjasnw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gbytsgwnc.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gmvhhlekp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gvhuywpts.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/grlooveip.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/govgygliq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gmzaikljr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gljlsvmti.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gygdimzqi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxwjljqtd.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gmqvkfjux.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gsvtocafd.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/ghmztthwp.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gyigtuhgw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/goqryppwe.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/grotnzhwc.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gjstpznoe.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/giqzbotyu.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gzmbwxqoa.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/geebrmgdm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gprtvwind.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gqoruusuw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gownwrhou.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gfpgfcrtj.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gmyljznak.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/grwmmiprz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gxvmkotyj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gitbpsjac.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gxkaustyt.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gijihjvau.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gthhpythz.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/giszjdwfu.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gbsgmxezc.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/guocmzldf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gmufnmsrr.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/glbxkxndl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gskqlpldu.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gfhmmqmlr.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gdfpnlyeb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gltxakuen.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gryhkjqck.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvwqgqdtl.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtvpjeepk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gquxjcsys.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gdpemeatq.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gpxdbdhsd.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/grfmmxhbt.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gzjlkbhdr.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggzqsqace.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gtavxfbej.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyrpirmnh.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggptzmjxs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gdppgarrd.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gyjervhlt.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/goivuloko.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/glmmfcvpr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/guctlbapk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gytazwyre.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gipiqofah.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/guvwbnfax.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gccntskjl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gvbjvaqfm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gyacmueng.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gvwctxjqi.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gzflqysdc.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gwjlahyir.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gdtffpzap.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gukmavvkg.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gqsurzatx.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/garegaikk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gujnajdgo.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gxwkweelk.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gtqqutxag.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/giobmqmwj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/ggxmofzvq.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gshwiifgw.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gdyqpptkr.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gfgupnhbw.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gpbbrqlcu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gcpwhhtyk.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gnpxcgoon.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gsddbgpeo.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gcmvnhpdt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gxuxnwmon.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gwtslwylc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gkyqtdiff.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/geaejazbl.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/grisabmgi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gwgyzauju.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gzwplkyln.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gukmlzyyr.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/goxlqzvoj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gjjfdfmor.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gtgygcmhv.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gzbtdwxfm.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gpfzdywls.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gpotzzmrs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gxepwuwwe.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gvtmbjden.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gsslbhbup.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gpuixrreu.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gbjhobnjn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gdqojcrzh.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gupoucwif.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfmhnmme.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gldzezqhm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gnfelsmex.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/glsccibnt.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gkhhiwnlf.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxhewfxjp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gyputvnxn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/ghdkupfpl.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gmlxozucl.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gogqjoxmr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glzofctgk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gypxwihaa.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/grsutqoqs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gbfuohlry.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gpkychgju.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gfrtgvfag.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gpudgffpo.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gzihgyfpd.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gonjeakde.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gngabpzho.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gtvaacvjt.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gojsoribr.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gvtyezjug.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gspdkalcy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gxgaryxix.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gosjyntps.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gbxzakfcz.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/ghfftvuop.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gtspqmgcx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gwzlcwjcw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/grwnlckjx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gftlbvbpq.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/grfdimmev.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/ghoodrvqm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gtkivfzio.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gqtxwgour.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gnpeabnsh.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/glxfhesyf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gaycqwnkj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gdwplrdnz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gunheztfm.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/govaawcfo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gaaxdrazv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gjtivexpe.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/govghdbtw.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpfbnyguv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gssrsogmh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gyvrriwta.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gyfyeqtxz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gqxutelkh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkmqkczgy.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gfaakafsz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyiivvwzt.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gveypwxpi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gdjngwpij.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gdpyftevk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gsbqvlsxc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gaqxevzvj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gfffzwsxf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gqulzfxiv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gpbvljnaa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gxkqchvlh.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/guheoywgz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gxhzmfpka.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gibkuvrko.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gbuwhmnzi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbgzuexrd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gbyccxfgn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gmscoatek.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gvgymbtrt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gnvmhzwoh.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/ggevwareh.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gxyjixesn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/grodmspqi.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ganwzmqys.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gzfreucqt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/ggplxjjxg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gtmcyrpht.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gnhzqatlv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gbnmpuvuu.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gbtxedryk.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gbkhhvnht.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/goglvsdsz.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gdpiinuck.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gqdpcvfks.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/glmbroelc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gyjaykkrj.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/ggvacctcr.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/giudryvfh.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/glxjiftpk.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gbgywgfdp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gpiadzsyr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gpjysdhbk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/grcegeueb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/ggzoqmlpd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gghjiwjsw.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/geqzndnbh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmlimczex.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gjrszcxjv.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/guzpgdcfp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gnfrhyuxm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gsvmpnulb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gwcaoeshh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gnirntfhr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/ghglpmnvp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/glwqleidn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gnvcirhfu.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/getkscdvs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gxyeobqwz.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gakkuxewe.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/guauyqbva.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gsfliukqw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gwsmrzwlg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gcizgbqyk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/guunskvxx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/ggzjufvle.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/glbgdinmr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gqvuddzpa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gflvbfkce.sHtML


<!-- 参考信息 -->