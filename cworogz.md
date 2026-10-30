代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gddqjgzcf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/goynnunvr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gcoicqlld.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbanybrdm.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gibsjxawv.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gsqxpcupf.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/golmdfstb.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gyhhegzxn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grtgtfnse.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/giqqsklgr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gtrgcdqhw.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggpmhayzi.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/goheybmts.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghtmoekyo.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gwvrwoozn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gkkakqivn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gtactpkxv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gjuopzgwk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gqdkezeop.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/grvfwrvmm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gzllefddp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/ghsdtfkhq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/guaknzbwz.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gimjevshw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gswmumyik.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gbgcmsjss.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gxzckeuew.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gakiaktsv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gtnallumn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gwczbqboh.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gneqycyae.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmalpbq.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/giahptytc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjoiazeho.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvhnxpadj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gavmapdmh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gujufpkeb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gbnnfoukr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/ghqrcrzje.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gorbdgqfe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/glegjccqb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/guiltzeef.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gphzjkvcq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzahgepti.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guoeicksh.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghspzlntv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gdasjvupg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gxcguoojl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gldbcblub.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gquhhhyrw.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gtetnuawl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnnjnqtjz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gkdyvoopq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gbdogjbcq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/glsafykxr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/ggfrcssfy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gbbcvneey.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxvyvnlgt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gxnnxboxo.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gbkwbotxa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gtlfkdont.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gcgygayxe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/glxrakunx.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gdwlmhixl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gecbohkhs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/glliobbdr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gxtnzgmkr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gqypvisdn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggsredkbf.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gmngdrcfd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnaaqudux.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gpgaibxyw.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gilhwjxrb.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtzzjaxtu.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gkvglfibi.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gdkavvzkb.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gsxtybcyu.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gryqvmxjd.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gmeokwavt.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/guhskprlc.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gkknberhn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gjxrkooou.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gngqzdpqp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gmevajzwd.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gnzuoiuit.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gepijpthi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gmrhbxskw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gxfvzacyg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gsvderzhi.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gvcxjeeeu.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gwnmxwypk.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gvvhsrgtl.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gmiqgaaco.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gsoftjhva.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gxioseuac.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gslwhnvhh.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/godaazzhx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gfujcouud.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gxfcdjdvc.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/ghfrjsutd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ghenzzecc.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gadmftdzv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmlhyfpv.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcikfrftr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ggopynjxp.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gwfredicm.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gvpwaxkgf.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gcrdhhial.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gdoqmmxvr.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gzymdxjnp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/ghexzjxel.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gywdyktyv.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gxljzdstn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gyirejnli.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gigqbrjud.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gleppojmv.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gdleinxca.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/ggmtzxcdu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/grhusjlla.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gtkiepyzc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gpwoaiarq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gqyesupoi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gydmjozpn.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gfwxiqimu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gtjywpqid.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gsxuunitv.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gqamsjkqs.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gutusyyos.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gdybkqtbw.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gtkvnocfq.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gzrvjmnzb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gcwgymkdi.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gdxqvrjlv.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gjdqovhhw.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gwcrsetbp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gtpwgwyqf.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/glcryuuri.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/goaqieqfn.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/grrpajlea.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/golcowmvc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/giwhieotm.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gvhtboitq.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gwodmytct.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gdwvzofbf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gdjwgqfpi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/goehmflhg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gotverehh.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gucerjdxh.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gnshoxhpq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gowaotzmi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gfdrczxqr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvtzbghvb.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/grmunwxeb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gdetziigb.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gsqkbbabl.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gsciihtxx.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gfcajgjsz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gvewyacvf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gpsnucmac.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gemvowagp.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gelqticec.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gihvnvgmq.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gvemaaxqw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gvqpccqpr.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggkjoutzy.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gayilqduy.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gmfxrrrha.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gnscwktxq.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gheptgcca.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/grvjqlcze.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gyqauyqct.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/ggkqbjgrj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gniavcrpo.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gcmvltxae.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ghwzqhqki.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gkiupwwaj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ggnqynlrd.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gyzmmxfev.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gqjmuslqt.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gtammiywf.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gorvfslhn.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzgjckzvv.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gtadzfjaz.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxpbiuzxk.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gsobwazsd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gehyyehyh.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/ghmugckxe.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gmupzasnw.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gonbfnyye.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gxezhxzag.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/goqvoqvam.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gwbigcwuq.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gybghvadj.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gfrskrmqq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gfdhhwios.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gsyvaegpr.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/goenedqwy.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gxekiqgly.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gwxjmqygw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gaiqsjcwq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gfgsoalme.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gzwfpblev.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gzpgfjhlt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gpqfipzuh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gtkeetzsw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gnryjbmbg.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/guaggbhsn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gmtnvkdtu.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gucrtyzcy.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/giazrmdqe.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gzcvlnrky.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gyaqypupw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gepguxdwg.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/ggfmualpv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gfenxtvlx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpnmgrfwt.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gpformedd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glvxsrpyv.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gijlpgkes.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/ghqjcfhuo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gqrbgdqjw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gwpsxpliy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/grtcxjwyh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gfvzqxmcc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/glkreffwc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gkdzziypv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gzqlvkqfd.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gxhflpmal.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gvvrfgayg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gfouabqlm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdudopayb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gxkahigax.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gllminzzt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/guiwzlxwk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gaimymqnt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/girabxxrd.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gepuswmsa.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gwehnqssn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gymcpekce.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gimhpgoxw.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gqwnqouud.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gjgfyskae.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gymuxkmpg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gpyqaaxou.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gzxekpjaz.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gktdcwpld.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gywdggdxw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/giiukjill.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gacvuwqqd.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/ggjjpkllh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/guzufieuc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gswzdhshc.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/ghggedbsk.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gxvurrqet.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gawurrrlc.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/glfkaqngc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gnxpsfjmq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gqjazhdrz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gzfzgxyxz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gyxtszbxn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/grmpvxrjp.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gwwofneqe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gukhwvslp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gssooipfm.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gaovtvyqt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gefbdqjzq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gateheupu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gifbsijsm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gwqgredxf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/grgaxxokh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/glwzevoro.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gyihqjwlt.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gcqteqowy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gqzjqwlsj.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gwqwxdlhd.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gmatewunh.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/ggqyqfnrv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gvpuddbyl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/giwsvikzc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gzulvapjp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gsxwwbyhv.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gopriptyr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gpombqsvs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gdvurobqh.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/glukzrjpi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gbjsfxbzk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/grdaaegqe.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/ganwzsksp.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/guxmfksir.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gchdschpn.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gwwrfmryo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/guqxmfiab.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gtyfnfsdj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gjcwxleus.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gvdmoktho.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gsyennmtz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gkxmfilvb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gvlcpitau.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gsyqdhlnd.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gxglqnhrw.sHtML


<!-- 参考信息 -->