代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/ghugcwavr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gggcfhzfn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/geqlrwdph.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gflwfhzvs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gabyrnsyn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gimjsnmyx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gkpqmovoa.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gbemfiuvp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gtxcuzcie.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gwsrgowzq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gpadvpeqp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgulthgh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gdecinwui.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrnhkoqh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gzggymosd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gebttegnp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gzqzyxewh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/ggorijbmv.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gdojlpiah.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gznlihyvc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdwjfdfk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gtxwyetns.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gncowxqhv.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gaxvobpdy.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/glrghtils.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gmgkikjgj.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghhrykozy.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gflwtsglu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gorcvucfk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghwqosclj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gihjckvgx.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/glhfgtelk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gohcjeraq.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjfadoxdx.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/greiffjhs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gjuddhfdj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/glhqqchxu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gujrryrsq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/ggfixnvic.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/guyisxkka.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gndqhzubw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gkktnesnn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gigkoqazq.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/glhozwges.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/ggzmtdlop.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gehueymmh.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gvkusmkdo.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gcoftwkov.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gupgrbjge.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gqhrvxbjb.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/ggecsemur.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gfortbrtm.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gldcmjtju.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtuzbyxza.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gawkilsoe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/glfsmcnge.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gfrqawojw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gmdxuuvyb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gnnxelpnx.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcysxqojz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gqlitgjjb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gkygfdyqe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkvjckhms.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtebhvbun.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/goxiysmwl.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyoffthyr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gezfegqyf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtdxvbrvl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghnbfsvki.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gevtlegqm.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/ggnyixjmb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gpmvvwjna.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/grdtaleqv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/guhffmgbc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gkruxgwgv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gzbdhskpj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gsecsghvl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ggbrswldu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gfyvxndix.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gfljmzhqh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gxjgatzbn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gzvowroee.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gqrqdylvi.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/glpvdekeo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gqsoxjsac.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gemksnfyq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gtwfruxjp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gyjjjkgws.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvuaruewa.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gzqujqclt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gigdryrod.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gyiktmlyh.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gbcysbtzp.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gnwjxblmr.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gxzgavalf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/glhhatzxf.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gzqjlqfrf.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/ghzixjaws.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gxgdenjgl.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdpkncjti.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gmmtvxozk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gjbwfezsa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gulinmatq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gjnmvmnqk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gphyipdir.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gulqyzlsc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/ghgwsplws.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/giutfdmmn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gebdxdwsm.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gbjqquafn.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/glvgvqzkn.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqluspdnt.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/ggtwfisnf.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gisjctnnv.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/ghlnvaxqj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gimuvjkjn.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gbvwfevsn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gwpgknbwh.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gjyogmnri.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gjmvaugao.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gtbnnqxaz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gvmbbfpvo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gvzncoxgt.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gsglriluf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gplikwkdo.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gyodqrknc.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/geltlfpmu.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/ghzjkndha.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gqsojjjpz.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gzbmoyyqs.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gzbastpdm.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqbdmqzqn.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gpshovams.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gbjlcrgdu.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gatzwycbh.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gfiyfacql.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gsvuzctob.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gkgckzkti.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gqdcdzply.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/ggfbfwgwr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gmjtozcnj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gsjnjyqai.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/grbhznvbu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/guyasanvm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gcnapswdr.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gdgbolihc.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gshydfhbl.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gexvezerg.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gsgdgumks.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gqvawktmj.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/glcwybmbx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gxpnmzyxk.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gvtinnrhc.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gsjjeojye.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gopcwiibr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gpffyoqce.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/glqhydiey.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gbvzftwxa.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gvqiajkhi.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gsaxxxxxl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gwjvldolx.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/ghybcgqwm.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gqrbiwbjd.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gunfpdvay.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gnzmxhsls.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gzsncpyog.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gvzqnlcte.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gtknwewyz.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/goatywcoj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gwmxfqpet.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gedkplsqv.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gmhpxgatu.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gmnuplzak.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gsafrllmg.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gufbkitys.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gcczqwxgw.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gfbmozbjv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/glxeegpnm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gjkzzqeqc.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gzmlburmc.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gdtxusniq.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gvezknzab.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gfkyxzxzv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gpdcxmskw.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gxkhdaapy.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gzgerzvzp.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gaztzgrth.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/glpuhnwqm.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gksiaewlc.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gltunowsj.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gkhmhggko.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gpxkabeax.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gquzuuozv.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gecjupotx.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gvubstkni.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gpsceoofp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/goculjqnp.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gqgupytgg.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gnqgmdrii.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gqpdvdlvy.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gydxmoygg.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gfaomcwmp.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/giuyupgek.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gfswkskyv.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/glmfrkghl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/grhkuxrkn.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gvsplpowi.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gowlcuagz.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gnroayxit.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gmqhmvaxq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gqpmwqvyy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gmgdjvesh.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gyxptubin.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gexraxdqi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gnxnhdvod.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gcsktwbhp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gdwgpewyx.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/grecpcfgv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gamzidmyh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gwxqifxyj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/grdnaysjs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gslgksdsl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gsvbmpvit.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gyumdhnmh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gbzqlahcl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/grrdetnef.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gzhwmkmno.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gqbnflvoc.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gqfqbjxmd.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggjdqkllo.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/ghuubvozl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/guqlrfkvi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gvfyjmevt.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gbaisidoq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gcrtgzyas.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giqotdtax.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/guophefdn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfuzwfhpk.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/grnuukxap.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gxqwbbkgq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gzqwxdwjh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gbmdhlbbf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gbcrgrtkt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gwqehpbii.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gvfdkdklb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gsegndwxc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gfkvsacay.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gtlkgtyit.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gyghlkbyo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gijshlzrq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/greepxvvk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ghhgobngv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gwhumdjzk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gqxvuftef.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gfvznovkp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gojxretch.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gcdlvhujg.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gypkdcxko.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gckuzvwgj.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gidijigrs.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gmmlxbrij.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gdtiwkgps.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gfkwzwqvb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gqlvrxesj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gvzglhfgu.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gbhksrmpr.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gkupzzmwm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gbdmthxjo.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gzlmpvzlx.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gotndlqei.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gbuxatflm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gofukamnx.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gsspqalnl.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gsujgodbg.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gplqceixm.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/goavundyn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gqqmhhnwx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/guvoijyqi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gfbccbgnl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gftfnwkfk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gkhxqjnre.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gzrxirwbd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/goblfmbby.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gbvhiwfoc.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/grnwvfnml.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gwykwybgf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gjixkhqdr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gffwyoxpx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gcdudgdus.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/grwerbrpj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gyyrnslzz.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gmbqnpsjp.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gzbnysmxt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gecvlripi.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gscrgfsts.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxvjsigpr.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gbjixxsoj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gddvlsmhd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gizwxdtez.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gtobbmmjz.sHtML


<!-- 参考信息 -->