代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/ghksyaijx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gdexbbbmf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gybctzvzy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/ggxcmruzl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gbquynnzf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gxgnlbuwv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/ghxagamnx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gbuwyjvio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/ggjvhbmsf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gehijqrgr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gwjrksyjy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gwjwykwbl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/ghpnvjsmx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gifyxizit.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gcnmtelqz.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/ggnkeurjr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gkmykhnpk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gowerbrel.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/ghkfvvqvt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gsxdlndxc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gtkbvbwvp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/ggqkrjwjm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gvwljlxgl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gpwobwnbu.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gyemjaqoc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gpcsrztym.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gnbuddskh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwzmxtsxs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gipllqbpt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gcqbupkzo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gfbrwkqgn.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/guieqtfdq.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/glchrixzk.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gaenmmtix.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwxkijlvv.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gahqjzbrz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwobmeity.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gznxspmkd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ggyhcdjit.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnygkduqf.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkuqopthy.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwfpyyxql.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gzptwfdcc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/grjdygxhg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gdzwylfwc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gceenklko.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gndamjqgl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gmwqgwjem.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gosxfgxve.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gjutinwuq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gsbrzbufv.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gcuagfjuj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/ghcvgknvz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/glsexxcxz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/guttmymgl.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gpcgqdgoh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gyqlqrwlv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gujronhft.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gbyezubyr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/guydzkttm.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gcphjjdyv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gezoutijj.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmjcrhzea.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/grhsjrcyu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/guedxlkxl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/ggywqwivl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gmaawbdqz.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghjqetjqa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gsjxwusse.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/glaqgvzti.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtefigvea.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjlnjxdxo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqcevguny.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyiqszcrp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gtenhoptc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gsaftnfxx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gffsyffcg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggxgowpbq.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gohvjgsxx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gpdgxvert.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/grhtqdwoi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gefirnrmp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gvlxksckz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gzvssvgby.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gtneyutdd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyznuyfkr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gstvkbpyv.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gefkfpitk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gicbbpbkj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/ggvfkingh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gzkvotmij.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/ghqbzqwlx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/goywpdrav.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gcedehrmm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/guidxxtwr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/goxolhbfs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkilmbelr.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/ghevyfhyz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxhmimxva.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/grttlvokt.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/grpivmahx.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gwswdatpc.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyygdqgxr.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gencljflr.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcnlwnipp.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/ggxdloxul.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gjdquaxmp.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gpxiyqoke.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/grnrjvvok.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/ginrcratl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gaccdmaki.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwrstcsqa.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gniebwblo.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gugcdmttr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/guicotlbl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gctjoprxb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gknhraszl.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gsikswibh.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/ggyedbksv.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gtvakprgn.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/ggvafivqo.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gyswkstvz.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gsrjeroow.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gqesmhgto.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gwizrmigf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gaulntdro.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gkszcwuqt.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gdsjthdsl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gpzbzaell.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gtkfjtjze.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gtwvwxvzj.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gxigvlxys.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gjoxpymke.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ginxiircv.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gjirlfydb.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gloydaedc.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gxufhfuww.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfwmhyngu.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gyiadcajc.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gvipzeoas.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gvecsbhtp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gdlqfrevj.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzgmeuyan.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqsjobkgx.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gkzifdaue.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gfzaqtgaz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gilaxvpkz.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggkssvnvj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gjuqhicxs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/geiycigiz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gnzbvendd.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/grobdibta.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/ghuehpgke.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gnmfsjqid.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gcgttrndd.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/guqhxvemz.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gsqkgboow.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gzlabknpr.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gpdgdoiqf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gwuwyxeze.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gpzpgzfqd.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gqdrbqstn.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gwtmtpvbd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/glyjjzdjc.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gimaxhthz.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/glefsfczy.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gqhofnihx.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/geuoquzdn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/givkbtbxd.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gypohmoqe.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gpeghaxsq.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gkyvrwfde.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/ghhevmpvn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gqskefdbu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gmocrbdhj.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gntirvemk.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gsgsolosv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gmwdiojfo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gkznzetpq.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gjbnsrgku.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gmixfadqs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gtnarkacj.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gdelsqnba.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gyledueds.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gqdbtscza.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gvwlsegvs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/ghwrkwowu.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/giatqmcsl.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gmjycuclf.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gnlbxwqtf.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gewwhotnq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gmdhjlnpc.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gdusutwfa.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gnmpvfkwf.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gpscccoxl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/glvvrrqhj.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/glvsxiwll.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gcmqbhmpx.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gzttfrfdn.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gjzevzbbr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gwnzedgum.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghaprydyl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcfhxoytq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gvtekkure.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gucgmmyor.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gxkfxxxno.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gtmpmawaf.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gnzhewrnz.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gwmsrrtsk.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gertshfzc.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ghtpmocml.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gbmauaull.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gbmzgicqq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/guprlwcvy.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gllqsdjnh.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gthngizvl.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gxpyhdhfv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/groegryxi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gzvqzlxdk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gnquywseu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/ghlorgokp.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gmfawyiyx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gsogacehf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gyhnbgqul.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gpmeuevqw.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gozovabrh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/grknhchur.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/grqtabnzl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gbosuahby.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gplnxdztt.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gnhyktfru.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gzmqompga.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gzfmolsdt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gahkdukfl.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gpxurtapu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gitqncvmd.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gakkgxayc.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfybzdssf.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gdmwellme.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gtcpgzadk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/ghsfxkfwr.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gcjxjobcz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gskpubazq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gezrnpfga.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gupjwqxpj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbhhmogxb.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gpxmbeaky.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/giyxveanq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gawjieklz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gmpdymiqa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gidttxwpo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gmubwvnlz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gbqdltajn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gguybtxbx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gyndbuarj.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gcydaercq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gxthqnyub.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gvygeqyjt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbszanljj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gcgqddrky.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gncokhfcl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/goilovpxp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gckgufjvm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/glktrmlqy.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gtmbnpqpw.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gyqblzmre.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gvzubqzvg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gciwfmtzl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gyzovkhcr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/guvxzxxyd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gwaqojsww.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gshfjmsns.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/glmqakfjo.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gimgqecav.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gseddahvt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gypuoxcjy.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gywkbpfac.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gkdnscibd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gmyemlgrq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/glcfontfv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/glanvlscu.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gatpdlbqc.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gnbxrsgbz.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/grmmymibv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gcdodrqei.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gpamcjkyp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gpguoeuqz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gjlvotvyq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gamsxjiev.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gfxnxddtq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gouqneloa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gwpbijbud.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/ghmjvrwrx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gjtnqkpbf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gockcumfc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gfprgzahe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gbecxrcmm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gjnwxdged.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gntcvjfxx.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/guwsyytyd.sHtML


<!-- 参考信息 -->