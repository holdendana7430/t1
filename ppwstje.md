代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/geziorgff.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsperkbp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/ghqmhvraa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gtvnymfgf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsivjjleu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/ghecfswtb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmdbccnm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcouzsrg.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gugukkmsb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtmbwcgz.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/ggiaeauku.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqblcjko.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ghlaaccvz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gwkegenas.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fanxiaobao.xyz/Article/details/gkiedtajq.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gtecssvio.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyboszen.sHtML

[F06] 删除文件
来源：http://wap.fanxiaobao.xyz/Article/details/gghxbptzd.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gyowtrkud.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gqodylefe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gtmnxvqhm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gewiblfrb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvpwczfq.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkehvbqyg.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/geenbtofx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqobynztu.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpphyhsc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gfesakrtg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fanxiaobao.xyz/Article/details/griluqfal.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpceybpt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/ggbiugtbd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fanxiaobao.xyz/Article/details/gwbfmfkji.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fanxiaobao.xyz/Article/details/gumdztere.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fanxiaobao.xyz/Article/details/gclgzrvxb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fanxiaobao.xyz/Article/details/gxlzppyys.sHtML

[F08] 遍历目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxbddpvz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlyfmmrs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjmfabtdr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/garmddaan.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gatmejqhh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gjbapzjlp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/geeyyqlvj.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/goplwohkt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvduwkid.sHtML

[F09] 获取文件大小
来源：http://wap.fanxiaobao.xyz/Article/details/ghvnrusni.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcpuowic.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbuuzlyd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gqakjwfvg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtctmlqa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gywezwmjn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxhkfhto.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaokfhxw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fanxiaobao.xyz/Article/details/gazaedduo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjmkgzro.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gosbabaoa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/glolpsoel.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gwkpttroz.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gjlwjqkql.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fanxiaobao.xyz/Article/details/glfwlyscw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gllkveuew.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/grfxeznox.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfddpllqy.sHtML

[F11] 复制与移动文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giqcvhlgh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtcqjodwp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguxfvaef.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gmqfmlrix.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbxerfes.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgorijux.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnydzvnhd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzburdhrn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpavqowyr.sHtML

[F12] CSV 读写
来源：http://blog.fanxiaobao.xyz/Article/details/gaupjwecp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fanxiaobao.xyz/Article/details/geysdvhuv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fanxiaobao.xyz/Article/details/gubkckmuk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fanxiaobao.xyz/Article/details/gkhnnzzzh.sHtML

TS:   // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyoneqwq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fanxiaobao.xyz/Article/details/gwivegkjr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gihejqidf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fanxiaobao.xyz/Article/details/gkgisenip.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guatlgnmz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljqyyrrx.sHtML

G. 面向对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiiwwxux.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikzkobhv.sHtML

[G01] 定义类
来源：http://3g.fanxiaobao.xyz/Article/details/gjsjgjlnk.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gknfafvwn.sHtML

PHP:  class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtcqviyu.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfpljxbop.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvuqcjccu.sHtML

Java: class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gdpxklgkf.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfodrbwp.sHtML

Ruby: class User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzeyotgj.sHtML

C#:   class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmtxrdqgi.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnzdggtt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fanxiaobao.xyz/Article/details/gkxhbunwn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzchtkofg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxfhdtgk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkrzhnksb.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxjhwvozn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqlkmbgr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvonmqzhv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/giwxnlgac.sHtML

[G03] 实例属性
来源：http://blog.fanxiaobao.xyz/Article/details/gujbreggr.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmzcfjca.sHtML

PHP:  public string $name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gyjrmdhmp.sHtML

JS:   this.name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpsgbxgk.sHtML

TS:   name: string = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsabwset.sHtML

Java: private String name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmbdyjnr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfyuqqnp.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkdlokjj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gndhrgbrk.sHtML

[G04] 定义方法
来源：http://blog.fanxiaobao.xyz/Article/details/gencokonx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydifmtnr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grqbyjrcv.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gobazzzug.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxkejiyro.sHtML

Java: String greet() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtazjfwym.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyhtzfsp.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gxocmviyk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvteyvlto.sHtML

[G05] 继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gwevojqwv.sHtML

Py:   class Admin(User): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gwfxshpwx.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsrdxgsx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfmofsqn.sHtML

TS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggmdichqe.sHtML

Java: class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdyfstxg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gumlboqbb.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmejmcub.sHtML

C#:   class Admin : User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpznihwhg.sHtML

[G06] 重写方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbfnykbl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvraizudn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gziykaiyb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghdysladx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtkmbdty.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gejedixez.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcrbsmjd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwopwoqgt.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fanxiaobao.xyz/Article/details/gatvmesjo.sHtML

[G07] 调用父类方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gboflosul.sHtML

Py:   super().greet()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnargura.sHtML

PHP:  parent::greet();
来源：http://blog.fanxiaobao.xyz/Article/details/govurohcy.sHtML

JS:   super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnbvejan.sHtML

TS:   super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gcetkpeki.sHtML

Java: super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gmqfeezjw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gywgafpbg.sHtML

Ruby: super
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpruwgxwc.sHtML

C#:   base.Greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gjpuxjjrn.sHtML

[G08] 静态方法与属性
来源：http://wap.fanxiaobao.xyz/Article/details/gibsmgzta.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fanxiaobao.xyz/Article/details/gumerbonr.sHtML

PHP:  public static function f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfdbkpyhz.sHtML

JS:   static f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glubclyey.sHtML

TS:   static f(): void {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoovbjxl.sHtML

Java: static void f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjfrzjbb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gzgigqgdq.sHtML

Ruby: def self.f; end
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxajvkjr.sHtML

C#:   public static void F() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvriqmfde.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fanxiaobao.xyz/Article/details/geunparcj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fanxiaobao.xyz/Article/details/gskwedtir.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gszhaisiv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fanxiaobao.xyz/Article/details/gmorkfick.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvrwywvg.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmcfkbwpb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjebwksol.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fanxiaobao.xyz/Article/details/gxhwvhnxe.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzkkdtsqp.sHtML

[G10] 访问控制
来源：http://blog.fanxiaobao.xyz/Article/details/gwzybgurb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchgzubyv.sHtML

PHP:  public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhbrlbni.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvfvuxfv.sHtML

TS:   public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gxxtzsakn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqrpzlgm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyanpgnb.sHtML

Ruby: public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gabanhiuw.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fanxiaobao.xyz/Article/details/guulnhoas.sHtML

[G11] getter / setter
来源：http://wap.fanxiaobao.xyz/Article/details/gbvqdxjiy.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gdemhwxzc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnoxbyqa.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhqbjlzf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvvyifcj.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbvpcpps.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwkyfasp.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsmhlqyl.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfgesrkqm.sHtML

[G12] 对象转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpnwlaau.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fanxiaobao.xyz/Article/details/guzftcnni.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glksnzsin.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghtbicwbo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstpbjcjh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndzeofnt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmidaubpz.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gyrfddroe.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/grgvefpfv.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcqmpwoz.sHtML

Py:   isinstance(u, User)
来源：http://baike.fanxiaobao.xyz/Article/details/gzcfllxnp.sHtML

PHP:  $u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gqhqkpmwc.sHtML

JS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gcvtxsbje.sHtML

TS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gispocswn.sHtML

Java: u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzxlkykn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fanxiaobao.xyz/Article/details/gqsfvmpog.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gupdnrwqe.sHtML

C#:   u is User
来源：http://blog.fanxiaobao.xyz/Article/details/gklcuwkvf.sHtML

[G14] 数据类 / record
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlzinyoc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fanxiaobao.xyz/Article/details/glppnpjny.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiihyhvl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fanxiaobao.xyz/Article/details/gzjzbxmaa.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoaxjnow.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvagtwbot.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/ghtjjkorl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaquqhkl.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fanxiaobao.xyz/Article/details/gkolnvoiz.sHtML

[G15] 枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorurmahx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/glooydhmy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkzelkleo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisvsyoqw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gnwqzoqld.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fanxiaobao.xyz/Article/details/gyhoeehiz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwppdeira.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxypmnwo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gfebjtrjn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gacmmumed.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqacasod.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fanxiaobao.xyz/Article/details/grepjrgxj.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gooigscuc.sHtML

TS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gwtknvffa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fanxiaobao.xyz/Article/details/gqvvysvfs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnylezldf.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtujatchb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fanxiaobao.xyz/Article/details/gvxzqlpew.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzxvqomkg.sHtML

H. 异常与错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/glsaccytv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkfsjvuk.sHtML

[H01] try / catch 基础
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiweiomb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/glnqynugb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjkkfbdi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gchunattt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqspmiwn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gexptkwbe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gtscctuco.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fanxiaobao.xyz/Article/details/guijjzsxl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gooqfodsa.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gaymkgxkf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fanxiaobao.xyz/Article/details/gjceqirwq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gttzeyqry.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxpphwny.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzdwuhalw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpmwwyis.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmomzvvb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fanxiaobao.xyz/Article/details/gnxvllzrj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/grzjixxdh.sHtML

[H03] 主动抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/ghlkmclpw.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkysnflp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/ggjbissof.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gclmmoibb.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gwtwkkebo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gomosjlvq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuerszno.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fanxiaobao.xyz/Article/details/ggflcbenw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gggfrsrri.sHtML

[H04] 自定义异常类型
来源：http://blog.fanxiaobao.xyz/Article/details/ggpymeonm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpwkmgpk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcireotlh.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/gudzlgese.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghovrgjji.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gudrqykiz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfdxojmq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gssfwxams.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glcvgsyuj.sHtML

[H05] 捕获特定类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjxumjum.sHtML

Py:   except ValueError as e:
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjuuqznl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbtsoyxm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhqowmnb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/goznfasut.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwvcnccf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fanxiaobao.xyz/Article/details/gwtxntqmv.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fanxiaobao.xyz/Article/details/gucmunqpd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfzuhrrn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdsbhgqa.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpomurmyy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gatobgjpe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdkhoyoq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchwlibow.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtejawkyd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrzfxebj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fanxiaobao.xyz/Article/details/gzfhdwmxz.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gktfjcvjs.sHtML

[H07] 断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmizmioon.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fanxiaobao.xyz/Article/details/graonamyn.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guesagfjd.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzfuwgbl.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjsklfep.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fanxiaobao.xyz/Article/details/gljymyija.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcacaato.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcsoznqk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gpmygesnb.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkiritbw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fanxiaobao.xyz/Article/details/gujiqzvwe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnwdcfsk.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqtrseaw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fanxiaobao.xyz/Article/details/gelketpbp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fanxiaobao.xyz/Article/details/goebhqvqu.sHtML

Go:   err.Error()
来源：http://www.share.fanxiaobao.xyz/Article/details/glwtguuje.sHtML


<!-- 参考信息 -->