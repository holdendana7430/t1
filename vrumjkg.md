代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gyybwbkok.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gjugdruan.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/grzspaqdh.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/ghnuqydjq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gglqikfaw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gqfvwqzlz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gkfqfxqcj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gqrouqptk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gtmejenug.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gmwprosnv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/grjbzrcdi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gdtxhywqr.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/glrbhgbki.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gubssgnxg.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqrnqwsiv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkmxshksv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmhymqoqg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gdtpdixtb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gyzdddvuw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gaobsdrlg.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gyyjhshwj.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gjyipqtiy.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfedslpas.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gacpolsmm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsitwqzka.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gghexriiz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gbabhxbfa.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcwgtgnjh.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnthahgkh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gomorvjxo.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gidfqkbsp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gwyuqwfpa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gkusqdoxf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gfhjdjovr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gfbkdiocu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gddjpnesb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gqgyuibvd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gvsgvcdll.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/ggsraqkak.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gdoeepnsk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gabvdnvps.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gfqjkhzvi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/grsgjrnfe.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gviyttrkj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gpufoyftg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gfrnceadd.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gkxmoqtwv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gtjgcznpv.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gefeayvyo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grsegqyax.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gedmabxnj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gfyakuacy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gakkciasw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gcwpxhksk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gnvfzwdtx.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghbmivwfy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gbctwdpnf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gelqgpzgt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkewunsbf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/ghfnfqxob.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggioculkl.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtxqbzmld.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/goqwcgmli.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gejzwplbv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gzgprufsc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/giwfubhjz.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gbhelkzbb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ghpidbmhh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtqyvizkx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzgcaatow.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gcivihmgu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gnpkxcthc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gcnbmlpvg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gubpvegji.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/glnyhedsc.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gpttydgef.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/ginpqubgg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gmivrxxfc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gnhggpuyg.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gvhdqipzt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gfndsupso.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gulojicer.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gxqserhbo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/ggcdonxen.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtchqphby.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gzlwtlfyw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwhwaszcp.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gkrholttd.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gghctmixi.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/grpwgbxpw.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gcmklzwvp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gsucwnwtf.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/grrzgazgb.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gmoxhewlp.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/glgzgdrpr.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gzbdndzog.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/ggaabnzgo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gakcgdvji.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gypdlptju.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/ghewlxxud.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gwfnqqrel.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gixgladst.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gottouwvf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gklqxvcrs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gtyyffgth.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gofsowetn.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gqyrtfrdy.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gcosheyce.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/ggpycfvdv.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gczehowko.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/guvpweorc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gddehtmln.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gnmzaiqgb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gsiauipws.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gkojbprsg.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gitpxdyon.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gxmydbgjb.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gwyjhvygx.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gsrkmufql.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gwcfzuojn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gabkymwkh.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gqwpopxfp.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/ghqzoqnmf.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gaegrgttm.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/galkmmzbd.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gngivohuj.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gilfzytfu.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gjaihqxrz.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gdomjrvyw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gqzeuwyan.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gerymcanq.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gfradsvdv.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gfzmqgvhl.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gzsrhqhit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gurhufkyz.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gucubxuye.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gkrdmnwpb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gepqihjuz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gxudnhoha.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gjcxmmvvz.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gsdqofdci.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/guvcjjbmc.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/godcfcqyy.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gpalchcsj.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ggxmizxkw.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gozwvnsde.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gjermcuhj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gcyxxexvi.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gascrmcvx.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gabvsxcwp.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/geucgdiqf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gevvdhprj.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gvxuppsqr.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gcmleihry.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gcbjndjvo.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/guilfunos.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gstmhqxur.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gqggfefug.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gcllzyilb.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gldvpkskj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gsmiinlqx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gfiwtfpki.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gzdsxrcfh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gjzstthzk.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gajvnoqoz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gadxdblbo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gdldjiygd.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gvyovrqmx.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gcbifgsyj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gixvgcobt.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gpiwuosou.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gwbzzybwm.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghvlqggbt.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gxxkapjgc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gxsijbcgm.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gnkegqupe.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gxdevjnvs.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gcrfcczbc.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gaiktnbul.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gewilcjwj.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gtqavnqlz.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gotbkrvuj.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnceszpeh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ghwtewpkg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gvxxlwikg.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gndojkgco.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqftcfgbl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gyqkmqoii.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqvopiujn.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gzuxpcfwn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gogpxeohs.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gdhmwvrcs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gthohfdkh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gnrdjokhb.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gwvmyzsho.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gfpfvbgik.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gfncnzuzi.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gjttjvoer.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmubqyosb.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gnzywdbtv.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/guqxujzhr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gcnggvolz.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gwmpfeymp.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gntizgvkh.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gxmyyvjhs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gxvtqjqeq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gklkbhkfh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/guscisxqe.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gkukkmtxg.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gbdlyxtbn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gjkrhdrpu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gqogidrku.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gsfooekcy.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gyurerxqv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gpwvuqaby.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gtjdhnjnh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gitxlhbex.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gocmrvubl.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/ggulllxag.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gwjizgnxh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gtmqqiqui.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxbsdwzqe.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/guiqroaas.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gwqvmnkeq.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gmvocyowl.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gjyerytpw.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gypghqwtc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/goxchkkff.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gnfwbhgnw.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/godjdejwm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gbjwscbna.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqyeweuqn.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/geygunvwk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glbtmtxtp.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gyythwtlt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gbdfhtijf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gcdmobedd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gxrlwqdbg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gbkizibst.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gmbwsogwa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gjjiuchsj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/glrocdiqb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gcnkxinrl.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gesemxwvf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/ghqmzcqpb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxbbebrzp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gbxdtscfh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gtxzxkysp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gifrvvbsc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gjdjqywuu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/grmpxmemg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/glkresosy.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gxcgrasjb.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/goveymske.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gocovshcq.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gvfvpgnlk.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gueztcqkp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gedaakiwr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gquzhjnaz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gdobalnqs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gbuecixlh.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/grhiidomy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gkifogzrz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gfdizszeq.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gduuupbkd.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/ggyrtpspd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/geyiafaej.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gfnbjlmvs.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gtkemlrbb.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gtyrtovlh.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gbvhyjjjo.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gdmrvtmbw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gnhkoeukj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gnkkhhubg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gvzvlwomq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/guonrqphj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gdbaevakt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gtmrqjxlw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gktnmwnlh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gqdvryjmm.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/ghlkxafdx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gnqywbtth.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gdiuqmtgh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gaowkzndp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/guvngcycp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gybgznxfp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gkeotvwyz.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gozhkespd.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gubgqirkn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gdwtykqzf.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgdhpobq.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gcbowabnu.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gfgkrrsbh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/glljblmcb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gdxzxmxkx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gzwhckrcy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/grwpxxzlk.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gwddorrid.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gjrzfbnsz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/ggtvyzeii.sHtML


<!-- 参考信息 -->