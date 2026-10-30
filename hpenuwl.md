代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gdomhzhaz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmqkgvpks.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gtuupfcxe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/grghppvhn.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gxtnzarzg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gruxwscjh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gehngqtlr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxbjiifdh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkbtwaljf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gmeboupfc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/ghfblgdov.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggbumhzgj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkbpxbkex.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gfzfncrtr.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gypbghxwv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gabsbqujh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdbszlduo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjhftvgiy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gtdakoybi.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghtmkziew.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gldikttcv.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gcjtxxiau.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gdwnkzyck.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gvxagtmep.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gvdjpdzvu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gchxtjhds.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ghyzepeqp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gdkegoimo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gzzebcrxn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gzfpjripr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gmiqlntqh.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gkleygmjz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/ghvfabkce.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gnuzvaigk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/guamhnkir.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gspqbaxbp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gsaxauhcu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gyxtcsogv.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gemcgpbff.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/goodsnvon.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/geoeodhwd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/goqdhelxe.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggtsyypps.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gjfqsuucp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gkfmgwbxx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gqwyatyco.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gzbjwfghx.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdpigjaeh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/grenypxqt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gbmtmpxhy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqzmdhaqo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gpcsyeqrl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/grrdzwpjz.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnybwzdvz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gwjwoywci.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqpaxyank.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmyjtjbkr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcxtwrlkq.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/geahxfdxn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gpovkhfww.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/ggixkvcxk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gekhynaap.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gxhxqbecc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gxbhmheig.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gmfmvwuhx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/geyjqovtu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gexztrzwl.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/grqdrwvve.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gmchvfirn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/goalgrznx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gstvgrxmb.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gabodpfac.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gxdkishgv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gbzhwnkcg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/ghqvtbxia.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gbpiwzoqt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkbzekkbr.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gpowumbnz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpuhfqrla.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gfjhreopx.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gqohsnyev.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/glmobghjk.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gyddzarqy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gmquzkahx.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/guzanxmcx.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gixvobfhl.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gretjhkyo.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/ggsovpyqr.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gljbwxauc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gtkdnegxk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gbuaaffol.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gfuyuticf.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/grpwgyrxh.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gbitfrjtl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gvleqzeli.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gztjfrsyv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gqiyvtxkn.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/ghvoeujqr.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gcarimzxp.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/ghebefnzq.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/ggpnjuwxn.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/ggqicfthp.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gzheuoylg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gztzomxtr.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gkottulec.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gpwxerqty.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/ggkklncll.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gupkshvkf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gelizhlow.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/giqjeuist.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gocqnewdu.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gkglwplin.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/glkwodpgs.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gbebzcady.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/glbkdutkf.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/govxipdys.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gqsmmfjsc.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gcpxcpixp.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gnwnklnnd.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gcgmqncnf.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnzpojqoj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gcsaxxeao.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gnmxaevot.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtxqzdzsq.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gjubknnrs.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/grsxwffps.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gacgpreuz.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gxghktcop.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdwglnbac.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gprrvqafl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gjucqyjxk.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gxommbbqa.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gqtwkjlmh.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gmzanjpud.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gmstsjpsk.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/ghekkmtne.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gejytqezx.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gcpcwqhqj.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gqbliwpfn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gtrbbrpot.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gufueiwut.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gckeekqyp.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gdmowrmgv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gghtyrivl.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gbckjzmzc.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/glxyuckqa.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gtupibtig.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gzzkmwhmq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gnqunosiu.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gkzsrotkk.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/ggrieqlpd.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gyfnvmikn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gsnaylpfa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gkfrpiiox.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gwbkjsehy.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/grhzzwila.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gvjjoqfvd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gqalfpcxi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gsnidiozf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gionnjfuf.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gbzrjpnfl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gqofchedm.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gvjdefjms.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gikvgbhxi.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gdnzzynpy.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gjjmzmzud.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gwnspcuez.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/glaohtvpc.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gztfrkznj.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gfhmldznq.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gfufildea.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/grwtrgdqs.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghyeqnqes.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gbkbtktoy.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gbywjdajy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/goveucqvq.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/glqkgtata.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gnsdbhzau.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzsubsrbe.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gzkajczsl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gxsaqxtwz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gcatfqyru.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/glekowbjh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gtqpbocwy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gydfyywva.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/geeqrhxjz.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gvqqrqvtw.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gyabekzuq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/ggrcwtmtw.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/ggzvataan.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gcehmuetm.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gcmlhpsht.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gxnlmkkkb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gyereswwq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gcontwfng.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gjgpssvap.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gmsfbocgx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gpafrsjzd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gvaewcquq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gusvkxuvw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gskvioffq.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gepmildpa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gjrpkxnnc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gflekihdf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/ghrghtupg.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gzrsjsjhd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gwbiaykcr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/greecpwap.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gmrpirszl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gdxlatfrp.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gwtchjxvy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gfhbleerw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gfeulfraa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gfrrvcwqr.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gunflawvy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gieanbkud.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/guvdtplka.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gnfozzdbp.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gtkjptcoh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gujwvrncp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gcvnmtgbz.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gfwixhmol.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/goleyfsbi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkmvivhxm.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gccikmhvg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjafdxgng.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gwbhmtbkt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gnchuvemh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/goizdchvs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/grkxbgpit.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gjmnnbtmp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gtmcphtdo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gxktsoqvv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/goctwlwrs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gwanjtcwe.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gsiotjzzu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gnitkpnem.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gvecnyfho.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxdpckgrb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ghpwpkkag.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gcloiwlyj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gqfeyvkiy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gaqxtsagl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gclqnojvw.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/ggqtxbczl.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gtfsjsgww.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gqcqkndbs.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gtozjeywi.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gkrpvkmbo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gunnlndae.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gpheivveb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gixeotgyy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmkxiqbpx.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gvcgmiopn.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gvsakyxpp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/grksvbwdc.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gpaluswzc.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gvjsoljvt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gqeouexip.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gfncuawzu.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/ghqpuattw.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/ghusjraut.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/ggtfyunpr.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gbzrokkef.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gghmsemoh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/ghcolfhct.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gqojrfsst.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gyswubxnp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gmllsethk.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gloxlipqp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gtdkecxvd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gjshvdidz.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gyvhmmsst.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gvqfakaey.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gzaaebxmf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gkznoqogx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/ganvvnbjc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gjirgtate.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gytybvilq.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gxabyiqoq.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gappaxllv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gepjaorza.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/glmzraanv.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gxpvmuzho.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gxekxgasj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gbdkszcyq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gqfpbytwq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/ghbmcyugd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gpidddtwi.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gohjnqbmt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gpxxcehcl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gjmsgticm.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gvienednv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gryatqtdu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/guyqsrxea.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gypclxnza.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gatxzsfjm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gbpawjrcz.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/glegyekue.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gpelskkwz.sHtML


<!-- 参考信息 -->