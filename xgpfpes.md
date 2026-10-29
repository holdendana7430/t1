代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gbejdqhrm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/glwuegmpj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gjopcjowz.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gpicbypar.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/geqsiqgbl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gnvfxrcet.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gnhkwjqkh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gtcfwirto.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gkequffwl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gqygxrekj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gdcutfqnt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gsvjcvzog.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gcgamesgr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gsbydcnzk.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/giigjshnh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/genigfpxo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyncebjvt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gzmosvvbf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gfyfctxtl.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gavocunxs.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkfewxfqw.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gffxytwbi.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyjbrunsz.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gedsdjekd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggskmnygq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkihdeqda.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gmaukpzib.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glmybrtvd.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gyelvrfmn.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfrxbwsgt.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/guctvgywe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gyjksrdjp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/grujkohnc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gnbqxsevc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gndsjpzpo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gppbidkit.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gwpvmvoxt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gmbxnrfoj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gbexyfvxw.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gcrybzclu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gsrypgizg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gknpwdqni.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gzeawdcxy.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gafrqnsdj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gwqglfmvb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/grxtdfbcn.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gdbhwfkwk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gmmrwjykf.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gfcnrmhnq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcfbqstul.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gfgyjafnf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gzdbgwfkp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ghtyumyvb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gyjnkbryt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/geldwrqho.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glozqwsdd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gggsprykp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/ggrftzkcg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/giptydsuh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gjmkgjnmf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gfjevbuvm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyspswohf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gqvzpuapy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpnkxbwqz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxxvfdxsl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gltxknzkc.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/grmgoajjb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gyrojwhay.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/grfgvehea.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gwtlpahjt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ghkpowjtg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gxgnsjrjf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gqukfhiqk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/geqpsinjo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gwgnbkbyj.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gokuitycz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gbofmqvii.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gmkextlhc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/guiztcmaz.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gwhrwhqvo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gnolrczlf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gvbecdlve.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gyigbhycj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gezpzlacy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvxatfyzy.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/ghyfcqcmp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gecplpozz.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/ghnrvfslo.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gfjbnpgez.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/glsuxsgfr.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gcyukxvyr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/ghmbhhbbs.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/grqqfypkg.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gxrfymnfs.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gtkgommhm.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/glejdekqo.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gshyxtaon.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/grekeqtof.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gesaqyrzh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gwftfyjsx.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gxvbkrdlr.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/glsfqlrsn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gneriewfz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gbyskhsun.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gzjafsefa.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gmevsvilg.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gjpmxcbns.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gkyccdrha.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gouuojlqj.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gszydmkht.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gvdzjmfak.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gbvpbousf.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gsqanhvso.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gjjchlyiz.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/geincbwff.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gqzkcxeho.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gdfzcoafm.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gecpkyoyw.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggaakufst.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gsagclavn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/ghpfefhmt.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gthhwxdbl.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gswjhdxlt.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gfzpdyphd.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gyutgjxme.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gnnpmcica.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gvaxtkfvr.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gtmxsuflc.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gsiyemasc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gelwmpolt.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gnnvkiqam.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gnhnirmre.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gtgokdvbz.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gqxculhjd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gnxwaudiv.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gixtbjsfm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdyctpgfs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gzgehcshx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gkxjmszfr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gisezemjy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gzeqbjnvh.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gnzohbcil.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gxvqvbmom.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gtjjetebr.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gnhgxtgmq.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gitbrwddd.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gujkdnkev.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gtlnehdsc.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gtrlfefje.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/glryxfwxd.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gcowncyro.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/ghanocenl.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gtyhbankh.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gbiqmdmkb.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/goxcboyrf.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/geuwevesn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gmgfbvrao.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gnfkhfmtx.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/ggurgamiy.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/giytmuvcn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gbuassbyx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gkfmneaus.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gtpqmawcr.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gicgvhzyi.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gnravxjrg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gymtqugan.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gllzhhvyj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnnlrjfnz.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gysjfshsi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gkvqqlbfo.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gcmegkzoy.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/ghaeqjvuh.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gfmzqjjft.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gswzabhum.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gslpyjomz.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gcnrxuwcb.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gpbsbphhe.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/goaratcol.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gqhaujdjm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gttsyjuvq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/ggqnxjick.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gccwbajfn.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gvxcgdapc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gwrglcycn.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gdmqrohzl.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gkszmhyuv.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gpjabfrwt.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/ggydttmhz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gxqtpvkep.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gzcjqdvvh.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gsoypwfnz.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gtmpffujg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gjknltzrn.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gosgpnuqn.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gicrvyuzk.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gevtxexdt.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gflnvminr.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ganvuxdza.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gxaxkwxnr.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gtavemnmb.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gfrvdaezd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gqfotdsxx.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gnuhhiswu.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gljsgflgk.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gayavkzau.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gwnxccoaw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/glrgozjja.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gplkikclg.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gskpjjpre.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/giofyjpor.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gcpjafkga.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gpfgamcuj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gpwayfzoa.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gruodzijx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gdunjcufy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gqbpaesgq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/grtyjfors.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gigantfia.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gdghgoezt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gljyjweqw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gxrbvkauz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlwrngmr.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gaqrxpnjh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gyzauxzpx.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gmqpufryc.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/ggzlfleqd.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gdpduelst.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gdbdlttcy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/grsoibqvg.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gfsbjvxws.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gggujobio.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvdkoqxoa.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/giogphdej.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtnbncrzp.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/goaaqrljg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gylkextmm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gnaexajbi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gapubmkac.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gaikqtwin.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gzufuyavf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gaoqxwwhb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gpwkmiaqd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gzpkktgyz.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gucnnfucb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gjbzogwiv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gwozimqva.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gkfkdfoaw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gdtpwcgpt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gerheznua.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gamepdjtw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gbgjpqowz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gadnrxxrz.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/geaceclzh.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gjwdnvjdz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gjxzxnnmb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gliutbzhn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gskkkmjsc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gtdspmkys.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gcclruyaj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gpqssmksi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gyrehrhum.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gecdvfrbw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gmvphpbif.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/glmynncvb.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gskndhbbb.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gwabcqkbg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/ghyjpojkw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gybbqxwrx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gtsvayapz.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/guahuutnm.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gylkpfndd.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gtbvjbzot.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gqpmvhlpa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/ghytummly.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/geoomioub.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gtshmjzaw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gkczhvyhn.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gqmzvbroc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/ggtnlmdif.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gxtjknfgn.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/glbbftzuo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gwzdkfwhe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/grtcnzqzv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/goigiuxjm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/ghvvzovpk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gvacrcetu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/goamtiziu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gxvtyxpmo.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gfaezwibp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/ggwyjeaxb.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gmsdnctnj.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gkwgnrefx.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gwahzyxre.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gezzcmiyc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gygiipoot.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/geablwjim.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpiradhuv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gtgmfnqxt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gaompicbv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gvnlzufad.sHtML


<!-- 参考信息 -->