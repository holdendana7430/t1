代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gooettvfy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/glpixupsl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gmbkolihj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gbhxyfbvr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/glwsqfjfi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gwhvvcjlh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gecmrzzbj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/ggpvyjvcz.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gfcgricom.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gyqzhpext.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gzdjwoqvh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqyugpabt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqszymblm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ghudrxanu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gatnghhxg.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/giqtzcbdy.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwqfnkfmb.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gkypxokte.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtxppvkay.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/grvefaatx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxarxxiob.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtdhgodhc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gkkzemigi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gohypwsby.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxqwdctud.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkyhrznvh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/ggvqspslj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/girqorugc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gdurrjhbr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gyqlgxqqj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gwtqfwdfd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gwwgjbbqf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gcpkrjeai.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gvfmahzbk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gfcirptqd.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gwqckrebx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gnczqlqnh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gsdfkzcmn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gexbjxgen.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gvzqcgtwc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gsmlfaffu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gvbnvxezh.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gsoysnulk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/grsftzubs.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gjsbyixwa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gryctqzmf.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpdjtogog.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gzkvggzxu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gvqvegvdt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gtwquwmoc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/glgfkrymm.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/giuazljpf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/grggjgkxu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gfjbzebyh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghodclhgx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/ghibcuzuh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gaubtdhxv.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/goizgfobm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/girdeqkwv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdjuwcepk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gysguzatl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwfbvfzzv.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/glhjlvage.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gypavnhdb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvbmqqmgr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gtbfhoymk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gpfwjgwlt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gopjtjsde.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gbdaagefy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfafrmpvk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gyxypiups.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gklosddiw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gtcykekzb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/ggyutrktl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gfyukmrka.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gwyrpwdnz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gsrgzbmjj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gmgdtowkr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gouihyptu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/girqwbqca.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdnhihpup.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/ghmygmnmm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwqebagkq.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gswhxhdna.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gftmbsiqo.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gmonabdgg.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/glzlordpg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gyhphseyi.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gchptvxcm.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/ghttpfwrh.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gkgjmmkgj.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gawticpkn.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gbhtdwmry.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gmbthgfbm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gqhrrjucl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/ghwknxcfu.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gopwxoloh.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gnvxypezg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gzsacavdf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gknnebjzb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gmivspklx.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gmonzlbil.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gbeggsexi.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gixxlnnmv.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gacvopjnf.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gzicnqiud.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gkzhgnnwv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/guuaawlxf.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/glutkuepz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gxtxstirf.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gexpmxexi.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gyyxtyvod.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gutwrykgg.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gedxzrtgu.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gtjevwqzj.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gixovpnbh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gsecxvclz.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gbpbsiynf.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gkroxnfdq.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gmmpykgfu.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gldqjjujh.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/guzdxmvss.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gtmrzhekx.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzgmkpzcg.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwghhvvwq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gjtyxmpvx.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gnftikeee.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/ggdejoiwe.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/ggwhzblhy.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/ghesyftkw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvcwifehi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gfwvlcvkq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gsrgzxjeb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gcqgycirs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/grttfbxkf.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/ghwcwkyxq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/ghyhdkvdb.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gmrctazfq.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/ghifmoxqw.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gqaqvkwmp.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gnacbkqul.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/ghrohzsiq.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gawxarzxq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gvpmaoieq.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/growmpgpe.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gafdurjsp.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gzhuudqyd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gtobachjl.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gdrqzzxce.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gffublxjh.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gupwfmslf.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gocczjipb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gixerpyya.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gugxfjhlf.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gvbgzejah.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/giqgujnmq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/goqjdhtjc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/ggdjfrbsi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gynhvvyph.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gtzqwuoen.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gjksmjxah.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/grvsgsghm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gqmgvtyfu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gyflnhovb.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/guomhvkby.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/givpznxfz.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gxbmnnspd.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/ggtsuuimk.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gbrcpzovw.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gbdoodlhv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gyfdpigrp.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gprcyeusg.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gimqzdbmj.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/ggsycngjf.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gsdwewizi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gqomomkaa.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gaxseubap.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gxkktqkio.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gsdjecjcq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gbweuxggl.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gzqpwusyk.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gwqrkixoa.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gqubcrvqo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gssldwiwa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gocplyyjr.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gzaftnxla.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gdlqozuhb.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gskjpnpcm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gtwynrkta.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gzdihgags.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gxrlvlifh.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gwlktwbtt.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gcrmunxpk.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gucegjopk.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gwiezhgks.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzujjyyqo.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gxjgjstei.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gbuqclusv.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gfgjjdzkd.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gdxuutlbe.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gwtpkkfjg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gomtzdpuh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/getxuglzv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gtjvsnrmw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gtgrfciat.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqujsymle.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gqhdovwek.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gchqlfgvc.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gdbmsxudd.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gqwcaptle.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gftrauqlk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gcarnzkvz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gmdqtgkbr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gwvapjckd.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gejbpiyjd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gfbnweryx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gllqohihd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gqymmtlzv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gcueqeaqm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gdjgrdxyp.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/glnchzlfm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gcmtxcmub.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gvuugbksc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gjawnceyz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/grzuzrvff.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/giisqgazy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gpdgvalzp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giyuiqjux.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/geilaqwsn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpahduzov.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gqxmjbols.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gislggutp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/ggwerwjoq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gnjgusgaf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gghenrcgj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gngepjdgl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/glrowxixz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/goqxoebmy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gpodvisiq.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gczylznnb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gzofasftd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gxlhgthdg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/grhrczhhj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gfpywjxoq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gtcemkgsa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gcrqdrlfp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gzapodnvb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gdatiftrj.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/glvsfiuyh.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gqeomenxq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gvsbanncg.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gjckdvwst.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gpuhxvuqh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gfgdamupq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gsljvhrrb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gsyewbdkx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gfnhgfgpx.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gpzkbbomj.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gwljsaaaq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gtezdrujd.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gxjvywslx.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gghpjbykh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gcxyesttq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gtmgaxkie.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gvssrfzsd.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/ggzhojtba.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gekbfilip.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gekrnipul.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/ggbagtbxv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gxlrzcpla.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnknmomoh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/guhnhpftw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gvipyjxft.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gkkhpicdh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/grplmbpfm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/glhpzwzrr.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gsyhahgcd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gveszhnlr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gqzgqwkzb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gzasewunf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gyvccqjtx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gqydfdqug.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gncsukiwb.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gqgnbqjsm.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gbsbhpxfe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gyuufmocn.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gpckpobrh.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/ghmqlwkfg.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gslidrfxh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/ghmypnrpi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gmyshnodq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/ggckbgnpi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/goxqknnyt.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gsfxbeqbc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gjpgvzzws.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gmiwpfokt.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gszcisdoe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gjckmdsim.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gukpnwblr.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gfqkiypie.sHtML


<!-- 参考信息 -->