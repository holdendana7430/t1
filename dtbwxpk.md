代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/ggxpwzioq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gouoiausr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/garylmakv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/goplkqzkc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gsanwvcat.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gkxosapjl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gkmrixkjh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gdgvvjtvg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gdkkxnupt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gszkvqdcu.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gafxohglz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggkzrsddg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdmmeyeac.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gkjbmekfu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gtxwlxkan.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjoadfgve.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gesixuisu.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gxjtnswbe.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvvhvdkta.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/giiqdcgnm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/givnpevgf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtpcjujtc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gcajelnce.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzgfyvelg.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grlvgkxly.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbphoptvs.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gkbzszfkk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/ghjuqnujy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gjxkkjbmg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/ghfsljebc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gjixiwxaf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gvmjepieg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gsmazbltx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gvvxvbxkv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gjietbqng.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gluwovlhy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gdawamewt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gchdumxsj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gdzlwknax.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gpirjvsfs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gzqqgqjpa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gprpwkpmk.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/grblvliji.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpbircels.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gkkvivetn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjzjttynp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gfscasltl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gmvulzlcj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gbalecjrf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gtxtsnqjp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gewubeudm.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gerahhzoh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gcjuennkj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gwmvosqye.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkwzcatrc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwgzrbnbc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzcvzjnza.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gidcivwug.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gumcklovg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjfuytuha.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwhrwtvvd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gbafrrqij.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gfwmrstnc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gvlbfzzpw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gzxnboocn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gaaptckrn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdulsosih.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzjsdudys.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gmdnjuyya.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gdbfrnnlk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/glyisazzp.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/goqkcwbea.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gckidtyfz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gbjvrlrmr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gmsdkrfen.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gbsmeskvk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gfaiseoxt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/geipvwznj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gnhyskeid.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gkjvgxxuh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggjvlwnvp.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gnffdnngb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzjflfthc.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gshchtujk.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gmweeslgd.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gipoaqpuq.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gryiomwss.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/glztkubrh.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/ghevhhtot.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gwqsfhepf.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/glwygbbge.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gieltattg.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/geadibpiz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gobqozvca.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gmcmsaasw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmykquko.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gjshxtoeo.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gcagllpln.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gtaxtvmjw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gzjqnsnac.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gibnsralg.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gsugirddm.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gtkbxdwgf.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gsetuxljx.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gjawkiryw.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/glinkvsam.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gbtbjqopg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gfpwekupe.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gbpumipgq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gqyaudkku.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gfmkosvez.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gmnxmvlac.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/grcvjbhql.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gklzcgbhu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gcnseirsj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gyhqwulxn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gnimmkbda.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gkvaasqiy.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gmbyitznq.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/glqdyyyot.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gareehamu.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gmbmdkwwd.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gizpkurcj.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/ghtkubtwb.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/giemfhfpq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gcyiislmg.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/guvdrbjvi.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/geanviolu.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gcebetvai.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gxvcukgow.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gxwoarmue.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gsmkbzaug.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/glutuarou.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gqsvfieqk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gvxqujvhm.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gbqqzazwz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/grssslgcr.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gwyltvwxh.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gxgnckkhg.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gbzvvjkxk.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gjqjkzhrc.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/ggafruqpt.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/guoxvahna.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gerrwdsgr.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/guodvpzxi.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gvvpjbtdt.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gboeuffov.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gtqliohvp.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gmmfocnog.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gdztbuewz.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gsthcumls.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gdpxwprys.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gmjehtkdf.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/guafwsrwa.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gurdvqmbd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gtpxcjwhy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gjdjfnadb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gminacyzp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gxjxpphue.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gildwwsvr.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gnhvzvoer.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gabbbjpcg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gzkyypvjl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkwnfetqa.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gcmkfnfku.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gnugqhcmo.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/grtdaxeyl.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gcgmlravw.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxuexxttl.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gdqihtzle.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gigcqllcg.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gbwtzzzys.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/grytuuzyq.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gxulxfmge.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gqqdqexkv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gwqzrzzlw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gamncdlrz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtisdxhgh.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gszsbepuu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gfkzcpsnt.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gzehpixeg.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gjtnanivf.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gsatjsxaa.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gznxofqea.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/giskjcmby.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ggymvvynh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gquwjjokz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gncfqdexl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/giwqoater.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gzvlusksr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gfkywbnee.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gdwxmjxyi.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gaqwzwkav.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gnyokgqof.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gwcapytzm.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gwpwpcrdb.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/givkkqnqv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gnrhrbubv.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/ggijufudw.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/grzmgahvc.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gbypeminq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/geqdxzyhl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gjmmplyns.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gmvgocjoq.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gxvnmjdvi.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gqckdlqjg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gizdaxkpa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/grlaxxmxm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gcfxmmbga.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/grsvqpfut.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gmgsfzffr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/ghednoyur.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/guxnjoqnj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gzjfnjafx.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/grspziklk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gxwxvxeyf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gtjbbhkwg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gihxcydqh.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/ggyvkmmgo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gqpigwxnm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/guunkszfy.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/ghfgirhce.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gycivxyoq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gclfkljac.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gdnkotedf.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gleezadkc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gwfiylcjf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnmorqrha.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/grmonjfmg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcipwbanh.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gxcouizvg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gekeayaid.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/glfbfwtst.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/ggjwohptq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhalfgms.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gzxgxvcst.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/ggzcvnfvo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gewgjkdae.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/glcgqtrwt.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/giyvezift.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gteilwfhd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggxjunkin.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/guauweaju.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gomozawrl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gwigldcmz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gpcobaeiy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gooilvnbo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfcutzjvn.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gpjrebtov.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gbtgzswov.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gihbkkjme.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gntgzigiy.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gzukakasm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gmwygyznd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gagfirsnp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/glqqiznvb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gksxclijs.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gnpnztulh.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gkmhgcure.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gooziexmy.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gvukunviv.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gpmvpkdty.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/grhyydhpw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/geddcnutr.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gddrtnejh.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gtkzebdgu.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/grpcqwsbn.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/giatpkvzt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/giyxpfepi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gglwqvgss.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gezftfwss.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gmgaafkvy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gouhghsqr.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/guealsarn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gxoqvjfvo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gqurwgqok.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gqklvxija.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gslsdtyyz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gcicetbhs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gxqwnegjw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/grxrvupde.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/glskofvza.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gkvahnttp.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gulburjbs.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gzmgpgcvh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gvjcvfajj.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gqxmgdygm.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/grgjgmfvb.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbdtayqvy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gvruhxnng.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/guijsquwn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gobqbqfoi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/ghvlxfiyn.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gqxxmtcrc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/guylbubhg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gwxgfncdc.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gklqjoyuj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gjmvtdoun.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/grhoznpta.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/goyeopmia.sHtML


<!-- 参考信息 -->