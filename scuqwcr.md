代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gtzjlbekr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gbabpujzk.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gqaedlgcr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gpznkqqkf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gbfepvwxz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gfalecibi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/ghkzjkthu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gbfdwnofx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gdhpmsobr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gunazjzmy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gejmfzrfn.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gynynrnwz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gcablcpsm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/glaqesqhn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/grckafdvp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gbfuulgok.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gbfkjkhdp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gkuurboql.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gpdvlpdve.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gjbndtmys.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/geozcaito.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/ggqsxajte.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gynoeyfzr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/guewrylnu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxnwyuahz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gmklkcyzv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gmqesbekt.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxnhtwhwr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gljnryvij.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gnbhkzggn.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guawdavil.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkirreikr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giosacafa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjyyyqyom.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ganuwcami.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/grnalnrbi.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqtylmneo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ggxobcbtd.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gqgzpnzxl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gfnkivfmc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/glvejdptm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gimnkawzl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gfykjqdxz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/ggwfeigyc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gyvgfltxf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gquoemlsr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gfqtlkcyw.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/ghztkpxqo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gpfkyqxyb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gezwtrxku.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gruatbfba.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/giugspfwc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gzdwzhzao.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gxjabpcyg.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gvxedhbrk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gsaaikmxa.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gqsvfcyle.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjzlaiuum.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/goqxjcxxv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gcjefdwom.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gzbpzhoqn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gjajvikot.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gjsojccnx.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcwudafjk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gmlduzgpx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gdrolvtfw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpuysebnx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gsqpuieyg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqjzllahf.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/goydmyvam.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gncxgtgjw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqbarwgwi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsegfwydv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gomnusvss.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gcdrstsjs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwfsuajjt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gltovlity.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gubbicirh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gtstghmcn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gymkyxsws.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/ghzqaivns.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gonswsqgf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/ghasdmoxf.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gsvkylwwe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gpbtbbyqi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gopxeqlcq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gutiniwfv.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gxlyrngdd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gvpdhmsqw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gjgmuziny.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gjdswyzeh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gaqnlcigl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmekycfoo.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gaaktdpqq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmhizaoga.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gedhzfyye.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gqgpmklxr.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/grdawhnss.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/ggrwzxnav.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gbrrybpfv.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gilwywwzn.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gdbtcumol.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/glptnhtdm.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gfsvqmzyt.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gktoqfipb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gkktffcyu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gmelfrgqd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gorirpjjd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gfwcfdxqn.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/grzrxwzti.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/ghypwgtmg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggnmlckbd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gsxnukbry.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gwembyqwe.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gacyprhvp.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gmztbejtp.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gpxxmwrek.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gdlwnnnvr.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gngghssmd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/ggivtvssn.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gekykyozr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gwqgptval.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/giittwopl.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gymbdacbb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/grvxzftud.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gclkecsts.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gmzzeykxb.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/ggtbkcwmc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gjblpzpdz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/guvnqnhje.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/glwaepyvu.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gscombhtg.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gcsdcqtpt.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gcokescbp.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gqnujxpha.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ghsjjcsff.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/giuetfbpp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/grxeahqsl.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/grpkiryhf.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gmyhgqggo.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/guytivqno.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gzhlvdawr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gewnrpbvv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gzrlczvan.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gmdrzmhnr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpxvdopok.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gzblkoxft.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gmspupxch.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gcazcykos.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/guwujjzhn.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gughmygid.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gxqjubxyk.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gxwehhxuw.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gjbtwsgmk.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ghdjlqean.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gisfrfbuv.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gxrxqzups.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gcnuofcgs.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gbryluzjs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gccuapvsx.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gnnhnjaul.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gchwovyqk.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gnbgsjyay.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gaadpduae.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gukpzqqng.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gqqgslmgm.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gjqgrnncu.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/ggojofsfg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gbjavtlnd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/geixcjfnu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gwuvgngvg.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gckkhgsjj.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gpudatulg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gxmqsaddn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gimrjjhyy.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gwvvdvsjk.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gxwysyaqx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gwjfnyhvt.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gljzksiye.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/geovnyqmy.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gfxsyndwk.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gmodzibde.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gmuyafmyp.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gxjlgpnpu.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/ghlnwrsyj.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gibiwduly.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/geowfcmft.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gvfrocuqx.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gvnbisyum.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gqfvrntsx.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gcelnvvof.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ghvgaetmf.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gncmagduk.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gihdjfdaq.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gpxnumtgr.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gtmicrmyy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gisphehew.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gaxxceuuy.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gldholjxp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/giaokyyhf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gqjjjobks.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gdavofexk.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gfzoqvomo.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gdetorrxs.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gdhduxgcf.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gzpknsxnb.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/guwveolry.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gctuhhzmd.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gaslvsmfx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/giyzmfrtm.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gbjlqxkdc.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gvknbmjmx.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gjslbcqrr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gkglrsalq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/guemqudqw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gvumgczbz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gailgisax.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gctkwzrxc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gxjrrjwxg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gxwvkhcrr.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gqrhnxjln.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gpdwywejy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gqysolsjz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gyymmlbjc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gexwwjder.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/glanndccz.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gdamrxebu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/geomidqnc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gufuitbpl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/grndjycrs.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gtnxdgfdz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gmgrzgecg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gwlgbxtmm.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gbrjsojhj.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gcfifkwqq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/grrmjgexv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gkfwztxet.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gswsidrns.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/ggrgnwepz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyeqdkpse.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gayrkrqci.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxddjyyyg.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gzhwfosxg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gisnowcrt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gfpgwssck.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gthunbeur.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gtrodbnbp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/glpqitkod.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gjlttlhaa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/grkggilwl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gvqgycixu.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gwndtwsrl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/ghoifurgm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxupyafxb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gcmsrlsql.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gknobalbo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gqnsjjjjt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gfgvlcwgs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/geiuctuad.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/glxmjxpgb.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gddmfvmvg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/glrcekiuy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gtosqzcwb.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gwvyrlfzv.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gloqypftp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gufvrdjkf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/guaknrrqh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gusbidbup.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gcshjykfv.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gopdlzxvs.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/grunknvdj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gpnufufap.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gjcjjjtvb.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gcpzufxqh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gjddgabrw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/giatoflsk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gntdvrvkh.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/ggpafzppm.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/grlsiwwqc.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gfsabmisy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gpifgcenw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gqjshytwo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gxhxhxewt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gzihapgdl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/giagcnhol.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gsyjtzhki.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gqjamccvi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gyxiwdfbq.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gkxwsyqrc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gfkuashsb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gfyqfsqji.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/ggdvutqjz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gbipfkbsr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gqobrqkbh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/ghezvpkfx.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/ggbmctqvg.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gljywlntg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/ggxwmxbak.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gfyarnmoh.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gslrhjtpw.sHtML


<!-- 参考信息 -->