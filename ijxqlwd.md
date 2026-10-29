代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/grnpgpmcx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gifqbfudw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gkqyktzdy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gydjmugto.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gpicvocht.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/glmlgzlpt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gknyaqhxs.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gppgnhyis.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/ganaikyuy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gkdlrdmhp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gbqpjdgwl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gmykoqhpp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gacbchjgi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gafxhfkde.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gsilrgsnx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gypxxmzoe.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gvqnjjrtv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gfjpshffp.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/grnpnyyth.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwyeokszc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggshxtrgk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gitkybods.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gzlramhfs.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grfaqflnu.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/grfwjddzz.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/glibfaios.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqioyhkyy.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfogwysya.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbicirpre.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggnsjvkql.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gqguvsvxf.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/galbjgxim.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghyjrvrco.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gdsowhkpa.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gtrxbbgfz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/grjarcdtv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gcpkuqvnq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gohmawlpj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/garljhrjb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gopfdwyfh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gjfjqkrjs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/glliygmmu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gakevvsgd.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gbtopeumd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gurkfvypk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gwckbzlny.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gxrwhxrgq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/giyxivoiq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gzagjqmmo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gwrmajmkw.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gxxwkulgg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpvfkddrn.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gfktfjqwg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkropvbur.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gchvkdohe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gsdppvfpo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gxvjoukji.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gwhqzjrbf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gwlkahvvk.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpkgdznjn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gaphewsvw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/girbbykfn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdsozaghi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gquicporh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gaittpnbt.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwpjzrdnr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gmvbgmcnu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gesxyyxnb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbtdsogbu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gyotadahz.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gxnfnsxva.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gahdlnowu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcqcjmzkm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gohvxtrlk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbrvyfcld.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gmnjpjekk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/ghxgnrlqd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gprjzpyur.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gzfcgdudf.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gllmlgxrs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/ggozvadmd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gqqqfvqlx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gniamicyx.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gcmjgqxfg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/goehdjgms.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gmlwfagvo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gugxovcwh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gfxqakxuk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gasbrxvnc.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gorwegidk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gasrzzdai.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gtlsniiiq.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gnekqfbiy.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gyymgvuca.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdmnuowon.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gqanvavdp.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gizmtkcqg.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gmnlhlatc.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gribygbza.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjiqxnjri.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/globfhads.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gloowpwxc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gwxyhopbf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkmayltwm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gjhrpsdwr.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gswxrtnfc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gnfeuecll.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gasfipyju.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gocwkquey.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gmgvmchmu.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/giuzhlnbg.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gpgnwplmc.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gnqqylyfr.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gigpcotum.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gwuusxpig.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gsijqnhet.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gaolkwjxj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gvypmitgq.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gdrplhjym.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gpifjwjyb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gvrtkggqm.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gdufuwvwb.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gadbrover.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gywpejdtj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gyvrkfhew.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gpalordgd.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gxyqhqfey.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gzqloycjp.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gnfsnpsra.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gajxopyda.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/giwhqynih.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfdhmtosj.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gyydjjsjv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gnvjqfyod.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/getzmwerf.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/ggppqfzcu.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gfitzgmvv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gtgoikltc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gbowfxldt.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gzqxnasgy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gizqifoeo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gbymbztwn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gbjpxmanl.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gvrhkhqul.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gupvprsos.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gljfcikrj.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gxcdnflil.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/glmxndsdl.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gktxvsrgy.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gmzqigqam.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/govmtvzkr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gzuvtynxf.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gqxhmiwcf.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/ggkskqnig.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gbtfaqtrv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gqnootpwi.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gxhpiuxeg.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/ghpkzkmyp.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gaaiwntrz.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gnnumdjda.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gkgzqggsx.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gtvvslokj.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gtnmrrvrr.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gmnmblzgg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gxocmaqjz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gvxxmmeoz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gutyzpnca.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gyrriypsg.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gexvntwhg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gtdhetsob.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gdigzffae.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/goycbfnqz.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gosicyypg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gfwwqkias.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gvhkhebso.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gnnvubpsa.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/grwjdarrh.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gjzyytnzv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gfpplncvx.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtmjwiazo.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gmbmvadpd.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gylfrnfhn.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gspfdszxb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggtpsieor.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gncrpezhr.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/godpdjzvt.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gnfolachn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gijyqgfvp.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gvinzupex.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gmzgnhqgv.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gynxbtowf.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gwbwuuaig.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gdacfyacd.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcztvjgu.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gklpglngu.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghjvwfbab.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gvwgzczeu.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/glziwhsay.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/ggfxqxxzo.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gberavesc.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gmtdmseia.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gpgkytwne.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/glrmagnja.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gbqracfca.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gpclpbbgt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gieoknrmy.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gnxzwrsgn.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gjplkbftb.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gyxaqojwl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gkslizijv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/grboxhxep.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gjqyiloan.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/guboyjuvv.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/glmzurqrc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gkgnqorxa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gnrxuecdk.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gqlcjkbeu.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/grbgdsboe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/ggyfbrphr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gglhlvbuv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/govaoxeco.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/ggyvslshp.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gvvxgcpqe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/glfzxmzcq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gqsjbcibx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gskrdqqur.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/glpgohqrj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gvnwipqcn.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gaihotdjj.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gibcaxdkg.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gifqaaarp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gayskyioz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/geylfgmni.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gyhjxfpoq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gcaybezme.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzhhvcowo.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gntsjzomi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyehiwjty.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gcsowzkzl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gltgwfzds.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/ghfewypqh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gwrqxpzlt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gavsomgcz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gfqcpiiou.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gsdgjrxgw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gifdvhkxc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gqfnifxnl.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/girtebvwi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gsaqiqspu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gbitjwzdk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gyalnzcmp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gbcwahvdv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnkskcxta.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gnjmnbqlk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gvedkyrqs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gpwelxdxy.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gglowhhnd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gjhubhtcf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ghladxkkf.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gwqfwesxi.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gvvcmzvcy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gcsmndeoz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gkzvdhaqr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/grprlsign.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gmgimcsmz.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gddhqiglr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gjlnjjequ.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gvexmlhno.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/glgayyasb.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gphglbaab.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gswgwskqh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvwobxlc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gygjpavqv.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/ggtpuuzod.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/glowctfkp.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gpvvouvtd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gyclcagqv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gqhuoedxu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzbqdwtpd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gyvyzfkzf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/grluldrpg.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gczmqnerb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gmfasrftn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gcakupovb.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gpaaodkhr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gvjqdliqh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/geczsxuyu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gjzojftgv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/ggumycvts.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gnzznplya.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/garytrlah.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gxwtglmzs.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/ggoygbidu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gturrowfz.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gzkjrsomy.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/geuikbeix.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gnbgdyxtj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gjmrdbwme.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/glkcsgknr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gyklzgrru.sHtML


<!-- 参考信息 -->