代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gnmtmsjxc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gqlqwlcgw.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gevywgcmr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gxlqzoxuq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gmuyjbndr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gfkvwcsrg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gdkbmnwtn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/grtmiroig.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gmegdcbgb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gkbemcwjh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gepyxhxnj.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/glvggjxnm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gbifgyegm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/giugrucoz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gwwgbixnl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gbrqtglax.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gkxrkoakf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gsfuggrzk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gpgywwxny.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gzusachuz.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gaifvhkim.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/guwghcorq.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcvonfqec.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxberfjrd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmhnoujpa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gbyrdivhb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gfgezwsak.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcrcqyedo.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnuqbxyew.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gyfvpunao.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gttxbeqsh.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grxvlngrh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbehsoeyo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghvskzysp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gdndfkqmk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glvkevhyr.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwjwthbhy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gderkklyg.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gadlpulha.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gypuyekxk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gjrlnunxh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gwwajiseg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/ggrexozkx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gwgllqwfc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gtlqupoez.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gcgdnmncl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gtxbeeixj.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gnyjtyxtg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gjojohtvx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gyxpbxgmz.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gvwgrezcl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gitoymdhn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gdbrbwkzx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gzsroieyk.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/grpnqoett.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/ggfzjpxcf.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gljbmdtvc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gszxiurce.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gffioxpje.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gwawxhmms.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gqcfymecs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gauzlebrs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gevejjbfg.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmdaderll.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/grrolqsss.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gcfpgkcuo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gugwjakwd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gntiqwpyp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gepuproyt.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gahzwpstc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gmmllpxcp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghnzsrnxt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gzqjkmvei.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsistkjwk.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gtrjbzime.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gjsbdxarx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gmprwmtza.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gslkqdorp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gadzftbyy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gtqrkzwix.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gluxnphqb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gqjtvlroz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gwonbsgjv.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gmphcatle.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gsvzxflca.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gjtgforuf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gswjiphev.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gecszwlce.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gnnceongw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gyxbfrhmr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gbjdztnem.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gurinoblz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyzyjrdbv.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gmaqgxsox.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gibpmyuok.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gunphdzku.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gooqodgne.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/grdpycumj.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/guqgxjpcz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gnwivtgfl.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gnatwynra.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gimhgvuby.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gelqvmuda.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxnwihmqf.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gjdcaaobh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gbxurwabr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gounmwqdv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gygrbsrus.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpqiwekmh.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gmdxwsgqv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gozmcuzcg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gtszynqma.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gtcnukmpl.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gzemhsmlv.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/glgjlhbea.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/golfijfja.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gsqdmtnkt.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gervgarza.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gcqennroi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gfepkpcsg.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gbqcncjow.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gtwbxkwov.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gxorhbzuc.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gwkzcicse.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gciooowqv.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grebcrynz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/giwplbgse.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gvesesudq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gyjcaccmp.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/glcxrvzvd.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gomnexoco.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/ghcsqqdtu.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gdkyxdvhr.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gzyacbozb.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/grsmthekx.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/guqoydwqm.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/giyrmoubz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gfsebksik.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gjvnmybkp.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gzcnqraqd.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gnbbxwoxj.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gomsqjlyn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpnxsuvie.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gmnfapkuy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gylnznpce.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goldsnljd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gwwrayjuq.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gwbheqrna.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gdxrbdvak.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gmcmecnip.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gppvfxtfc.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/goapyvexv.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gncheisgu.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/girngdvyr.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gvhdklygf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gdyuwiwaz.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gcpjdjuyd.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/grigcjulx.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/ghmswqqsn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gtsealmqa.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gxhufqbwt.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gjlfussju.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gndnypvnj.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gojalsyyh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gadnpnxut.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gpxehobii.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gslmmtbqx.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gublrzxbk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/guwgquzkj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gyoywvwoc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gnfugzxvp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gtgdjfufn.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gonttxkwe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gesndglkw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gldwpgidt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/glyimueeg.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gjjztjkif.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gyjegewsk.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gfytxuewq.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gfyvaostg.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gmufreumn.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gqilcxnti.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/geydawava.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gtsjpdfce.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gigfgevmy.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gxsepbovb.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gcocuiuyh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gtrxxutau.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gqpwfbceg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxqggxga.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghuacwupk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gwlazimfp.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gxfsfiqal.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gbmiofgod.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gdkxknill.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gbelaxxkc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ghleoopht.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gzdfpizyx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gchemegbh.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gudgshrme.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gzcjxtxdx.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gwdpqtqzw.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gdclpclnr.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gexrblaaw.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gfsoakxjt.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gzkowrqff.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gzhdhjtca.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gcdgoifbt.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gtjandnkn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gvqnsfxsk.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gwhptqaud.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gcgcpelys.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gjpbdzcep.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gbbfgejem.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gzgydqavv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gdjhshnkz.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gsawfwbgy.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gvwhiwrnz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gippmwprg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gknyjljct.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gxnypnysn.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/ghxvaovdf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gnicpeoeh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gaawitehh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/ggjoeweoi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gssjorzhr.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gejnzeswu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/glpgcqibh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gjlwehmrm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gbiamcrbc.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gsidqslim.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gxoxvqmsn.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gamvmgskp.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gjymigfmf.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gieboqkeq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gnevokgbh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gjneyijoa.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/ggtlommij.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gzbefgykt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzfmjlxip.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gqfzoujgi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnylxpfbu.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/glxbfezmt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gtjxpeplp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gixwwwycy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gfbzwghbf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gwcpwpoub.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gdkjzgqdc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gtpucaecb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/giepznldz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/garuladog.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/grgjcokuz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gquzhzeei.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gtehiexks.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gmputabio.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gptbhtivy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gjviatsyi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gtlomniso.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/glaqapnen.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gdkodeivv.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gdhnumzco.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/goxwlmbvf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/geijeyejs.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/geesufvoh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gwgjehhdf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gkzupsszl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gmnjgthzt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gxevpgcdw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gmarmkfia.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gjfcpgzmo.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gepbjthhb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gdfxpryqs.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gbajqxhcq.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/geykzreia.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gcstvlpmd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/ggqnhiuhy.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gyrpwucqg.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/guhmradiy.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gvcidoths.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gjsbmdzfl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gtqalvyhn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gvwwhhmcv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gpiqdguqc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gbarkojeo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gqeakmiqu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gjqlvugdc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gjjdrbdqn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gcrxhhezw.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gylshdiuj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gaswkjvyu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/grfepmfhk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gmxhnyweb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gphjledxt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gwulliwww.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtujapned.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gcwnqydmh.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gljlwsvle.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gvalrzjas.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/grnswgldq.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/glfgvimru.sHtML


<!-- 参考信息 -->