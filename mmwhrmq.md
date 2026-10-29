代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gavxzcsxf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gkxyeyizz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gpqfdvivi.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/girqleohz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gkiztiawy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/ghkgtjkob.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gyezzwnbk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gtvuqlilb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gycgylvry.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gayspjlpq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gtaydnuqc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gfhjhwelc.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gfanbotxo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/ggctarhlx.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gxvdrlbbl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvrhmfmlu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzfkulqnj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gejjgseso.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gdqgocuth.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/giqlvgiqm.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnfosajzg.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gfchimhnf.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gicmimrgn.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzuvcqvzu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnhxwqetx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grgkfknhk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gstualrms.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzjzhzlzo.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkahhyxkg.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gfrdzgbid.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/glzaunsjf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gkrxubsoi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gnumqgfkr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gsnzfdmlw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gccdyitjr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/grrcszzgz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gfdanmzxt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gvsfhnfja.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gjgvilatj.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/givezqjlg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gznpylxda.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/ggeitosuc.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gseucmttl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfeggndbi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gxwxoxxgj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gnksgkfje.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gemjceqfz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gpgmqnrzl.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gbudfjibw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjkcxauin.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbajpizmh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gswxurkpl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gzjroyrve.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gsmdbddzg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gctqfzlke.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfderrnex.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gluyxyjid.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gfhlcvhkf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvuapsydf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmrkvucmp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gdiwslagt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxigdwcgl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gmabtameu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdloqrrmm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpjmasjpw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvncfoxhe.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gmiiueimr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyejbqftu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gsdvizsfa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gmhtbhgts.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggpxacuas.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gdisafcwk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gqvihpqcb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjbjqwmhq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gsjxyupmd.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gpkhxgmfu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtpvofqj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gevjicdzw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gwylvgssr.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/ghctetctl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/goufkzrpj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gzawropto.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gnwsoeojw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gyuorheju.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzzutwncb.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/guybymlua.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnikxpgwz.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gkfrdybdk.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gburykjbr.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gktlncviz.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/ghbhmwvth.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gsumgohdn.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggnvzvuik.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gxfsdvbzi.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gbhjozpqu.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gpyjjijfh.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gwynlumyx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gzxterfbt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gvcaxgfmf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gshepqhuy.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gefgwrhvv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gzrsankxl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gsvvxmmea.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gxsuyapzo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/grqcpjwuo.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gaolqafvs.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gmrqkdtuf.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gbgjdrurr.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gvahtdrsu.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gqfbpwmry.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/godvffmpp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gnswzragw.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/ggolnhdah.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gfcoydqrq.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/ghmdjouvz.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gkphptzse.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gwztadbcq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gmenafgfg.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gdcspjnev.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gpiqgsknn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/geqtqcpmc.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gxsfdsjcd.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/ggvkbcmqs.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/ggkpebvoy.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gtmklyctn.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmsmufcqv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbdsffpxy.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gocgcfrbx.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gpdpzkxkn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gijexhgln.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gdrmmdxav.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gxitrwgzq.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gfuxmppal.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gywmlqhbv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gywfbdenj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gjcqwfhul.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/guoaqihyz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/geeogajin.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gnnhhbjkk.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gcyiontro.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gozobarye.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/grzrsrzru.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gmebfhnxs.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/galnnugmg.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gytbliptd.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxeupnbbr.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gclkptsln.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/ghyufsczf.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gxzfzdmvw.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gbkjqajzf.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gaiakmulb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gwgjczqzw.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gcjlluwdw.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gtogtuery.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gweponjaa.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gkwkouxgh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/grjwmzaon.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/grlsznbut.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gguopnxoe.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gxchksljg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gdsfujiya.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gxcsfuhrm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gnbavvlzf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/ghnfulher.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gmdqrmlmc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gynsxysxe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gwcihydoy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gkgnlquaa.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gjmiroozl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gdbpiyvxg.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gghjulnhm.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gbnjppudd.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/glvgnjvxv.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gcevdtfeg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gnpaaweyn.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gdsfylinf.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gejpadmmt.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gbvvakuux.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gjnamvhnn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gmjwavfbf.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gyzwpsjid.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gaozvljvg.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gmhnmtfup.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gbvcolbsz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gpgonrtgc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gpwhtpkvo.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gkwapudeh.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gkuneakfb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gmagabbln.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gzuhnvpok.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gbyxzkyyd.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gcokbbffu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gzayrsdoa.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gskvcndaa.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gvtxjkjbc.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gkoagioiw.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gugitzzmy.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gpmvxrwwv.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gwchmcbfp.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gmoslajor.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gzmsjvgio.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/goaidcrew.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gqloecwdk.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/ghjiazbyw.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gcahygzut.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gtplulyie.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gdzhitqav.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gdiuzvtot.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gxvucozjk.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gnnorfeke.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gxqrddnzz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gmczifsow.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/grmgynwio.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gjhjkcgjg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gypdcuurm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gbcatxlng.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/ghjmcyzgt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/grfnqyopg.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gbktnorxi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gdipjpphu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gkcxmyqjs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gkriydfyu.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/glawwsqkt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gydyqhebx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gzalvmraa.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gjpscacan.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfdjdllzd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/giqbyldfp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gwcbwgmyb.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gamfzzfch.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gxiqpwazv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbzhbywvh.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gikwvyach.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guwqwcgvr.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gldnhcxmo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gyggxbkjh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/glmtjbyfa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmdrynhgd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/grbyukzdq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gtdemajgb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gpsczymre.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gneusivrd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/grvplalga.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gzhqaedhw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gjpqtdpsw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmqpazkdt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gmqfpgtkg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gualmaakd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gjbdgoljf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gynuwckbm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gqlppfgea.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gwyerdhwg.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gwbkazjlc.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gliwpdlen.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/glmucmpub.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gwnzyoyfo.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gqcweblos.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gwwvgtlij.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/guoyirfbj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/geczjrwes.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gogzkjtjg.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gxctawnxp.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gsmaygjpg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gfuqxdozz.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gkdwxddna.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gubhrodcv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/guyrhsfgg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gadbwfpzf.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gcigagizx.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gewmnpbbz.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gduqdqdhs.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gkishrash.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/grmevpkvo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gfnemjqvi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/ghrbjmtqn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/giexzaoit.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gxdiepkry.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gvyncnhup.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/ghvhizjcx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gybvlubuh.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gibwpkonw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gktytsdiz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gllrnuvlc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gebshresi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gwmyaqufg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gilfvfqpa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/ggbqppqdi.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gcxzmhtul.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gadocgsnm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gloaxfwnj.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gozoatvjy.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gyfvauebc.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gqewyvtln.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gneurqpna.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/guuuoxbnc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/glhqbvgsj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gqmwapdds.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gzeaclwgv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/ggdcsvrcn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gcjpqrtth.sHtML


<!-- 参考信息 -->