代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gnikjqhpy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gcjpmcupp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gpbcomryq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/goxwhyxbk.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gfhvlfwcb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gpbbmvuhs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqqzbwvvc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxduviupk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwpujqxbf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/grqofagey.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gyebhfwej.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnbqxjcao.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnhyozsbp.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/ghlhoyhoo.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gchjkcgsq.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gekhnlyub.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtybuxwkb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvbwsbrur.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/ghhykqjvd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzhuihcpb.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghyqlagde.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gcklgfucv.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gioqjmdfi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gvbpgvbzc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gjfjvblgx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gqzvotjuz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gxjlhcgem.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gubeeuqky.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gmvceqzyw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gtrcgtwgh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/geiujasla.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/ggterbvnd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gbqeatcfu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gtqgzysar.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gmndanaxi.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/geybhcjxt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gxbyphxje.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gpwdggcmd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/garquzing.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gdzvmrkhh.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gyoncijrl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmuvdqoro.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkwolrntz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gtzfbrvrw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gshkhitae.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gekmyixhe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gmfgienuo.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmguxcdca.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gnttzjmrs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gfpqsfaqt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gverfwhwq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gzfteelbo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfixitttt.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqahixspt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gsnlvpcrt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkwywmbzg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gxicuhklx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gehtevxsl.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/glmzsxbof.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/glrusgkad.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gtwutjdrg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gmzqzqcrb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqqqekhrc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gsdygqqzm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gqilnhqol.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gzrmptqyw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gpprknveo.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gltljbrts.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gxiaygcnr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/ghwjivixd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gnecudasl.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gxezqrngm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gugnwytjp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gflpxzxgd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gaysimjby.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gszcxtuxv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmybhxwbr.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gltiboloe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkyjoxtiq.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/ggargkiyj.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gcrvratcn.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gctgnepai.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gbyptdznd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/glamejrwf.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gkajmviot.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gfqhsenep.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gkhuwzxfy.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gerxwsizm.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gyllczsri.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gkkhiadig.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gzizalcir.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gdgjsdlfk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvdqjsxbu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gyybdiuhd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gvebnxuyr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gjzehywmv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/genzeibyc.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gfatcmkxo.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gjclhndvm.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/ghjxpkvwj.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gnhyjhuij.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gjwdvixwn.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gnlaitcwy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gzlbxoiia.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gnxuzzipj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/glkieyudr.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gkbxzgvvu.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gwtzcmwnm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gecwyitsp.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gwbxqzqgh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gqlcralwp.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gwcszwrmx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gfodahevg.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gyybxthnq.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gnhhdnurj.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gcxhommad.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gmsutvmsa.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gthvjglbu.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/glefjlcwf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gcliksodj.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gzzomtlki.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/ggsaxfiwt.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/geenfzhzn.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gzkumegvp.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/grbehvqrq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gxvtgywfc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsqlnvyto.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqfjanvjw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gfcjwbnns.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghqkrvzay.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gxsuxmjav.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gslarazdl.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gudowwxmb.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gsxrubpvo.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gtbooaqgp.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gzxzmmckq.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gobnejrwf.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gcwyugubm.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gnlktpjli.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gbxgxjwtd.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gzvspqmrv.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gslfhueyt.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/ghukyxaep.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/grdqrzrei.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/giqhyaquw.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gxcexiehh.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gskivskih.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gjvflzieu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gnzgnjqxd.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gimqnwmqv.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gvzjfzcfc.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gkllvolzm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gnpnhdmuv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gzvtjjvno.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/ghqoqtbgr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gpqqhspmk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/ggmoqztcr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gujvyvsze.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gouzbgrnk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gkuquryxz.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gsucjofvt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gsisgzuhw.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gwoetlqgc.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gsqqrlltt.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gjfbkkpzw.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gxmkrunkf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/glvzuyona.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gdetvdytz.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gldxsuoea.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/ghskbvcqn.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gsqcovetf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gyikbojjw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gmrtdmzzi.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/glfnxplto.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gqulcnnkh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gxlvnbnhs.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/grmciidaz.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/ggiequoey.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gnmsjrxvz.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gibovntei.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gcjuvvbcz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gmgcwctzk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvexlywlu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/glsxsswfj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gvbqaktrk.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gvhrqozto.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gmiaobajp.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gprsxhmvl.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gyxcehzpz.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxohqzxit.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gadjwhqgo.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ghpocomlr.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gmcgoetbi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gqabkrxbn.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gdnnwaake.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/ghltkwjqa.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gfcgwvoxy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gvnmdmavg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gotttjdhx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gofduaubn.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gwwerdrjb.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gloticqqe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gzkhpibkx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gdzknanip.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/ggtapsdoi.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/ggihdpniz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gmtxjspus.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gsomtafvj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gfzegxgma.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gfghzjtox.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/geoovbbic.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gkflibzvt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/geuuvlhxt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gunafdqkm.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gtjzhrsvv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gekjvknfz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gbryuuron.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/glyhthvfw.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsfqxhpi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gjrfhgauf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gtjrtsxec.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gfpjrjwkv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gupcbgfrf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gftnbnopg.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gcjgoejqm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsigmzopu.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gsbpdmuzv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gbjxankyl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gkddfylvw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gsvwsvxoc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gxbhzglji.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gbhiwkgeb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/ggfejcpqn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gerktapel.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gjdugvllm.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/ggfqedips.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gswxoivdl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gjsxljleq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gttcrszui.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggnavjxbf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/grkicgyil.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gjurwjasn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/glkrzuwdy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gcwsqfuhm.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gznsduhku.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/glzxjioyi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gueylaete.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gxhdqgsyq.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gmiiwrftr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gowthxtzv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/grdylwaqn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/grrmixars.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gwjqeqizj.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/getziymlc.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gocdkhnjx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gnrbtjilc.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gqyohcnyc.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gkdcaznfl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/guhxwjyqr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gyyectfog.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gxusiefia.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/ggiazzhrj.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/guotshpxc.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gzscofdsc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gisgstiyv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gfijxwxvl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gjcmdgfdt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdkfoessa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gzppwumcu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gsqdqewlh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gzalbdnvc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gyyiwirja.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/ghesqeztr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gqostjgfo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gjtqavvbe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gqmbdrcas.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gxsikddce.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gxywcijls.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gpkdgiivp.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gfntdqiiv.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gjrqynwoe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gfbbllbyb.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/ghzpswopu.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/guyznrrrq.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gsekqrwgp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gufaszows.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gjxrwxafi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/glzqjgawk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gfzhbpcwi.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gjquyhgei.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gumkaezgm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/geqyejteg.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gfctivupb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gakgvgpfa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/ggjmmvhoo.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gogctdejc.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gsbsiixhb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gbehmynle.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gybralwho.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gafwwjgkh.sHtML


<!-- 参考信息 -->