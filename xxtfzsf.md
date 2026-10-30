代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gxsbzopxy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fanxiaobao.xyz/Article/details/gqiekzvpn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulvvvtno.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxanxfkyd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxmfrnin.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gxnvocbmz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fanxiaobao.xyz/Article/details/glicuaduu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtwuwmag.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvtqxztf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fanxiaobao.xyz/Article/details/gzfdtgfqm.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/glqqmqxiv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoiejlmn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfbwzrer.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbovwjurr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhhnooeg.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gwuqpsxra.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gngcxaxlb.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvhwdante.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gkcoutftv.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulygyjsu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gwwsvyvzt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gifxogalg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjkmkrqg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjedsgef.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gummhwdjq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwntrfkd.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fanxiaobao.xyz/Article/details/gyfwwbkgi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gemtdslsh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpvjedqd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gmyhskmtx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmlurchs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwdmprza.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpuqiwyd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmcmivps.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fanxiaobao.xyz/Article/details/grcqdfebp.sHtML

[F08] 遍历目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhezundl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzfakpgr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmjpviuyl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoicjewx.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjfubuyq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fanxiaobao.xyz/Article/details/giqjajscy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfkqbxhy.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gyyeitnbp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgbimctg.sHtML

[F09] 获取文件大小
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsnfvoxw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgmvuvsx.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/grctfgwqq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkkaypof.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonucqvom.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gokhyoasn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fanxiaobao.xyz/Article/details/gmdmrwhkq.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrcfvoob.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fanxiaobao.xyz/Article/details/gbbxlmdyx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnnkmygz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmipxatz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzsuuvqx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmulmzwsf.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfguumaax.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fanxiaobao.xyz/Article/details/grkjkpfwl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gwnrgpppn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gkahabyfs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyqipjcg.sHtML

[F11] 复制与移动文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxpkzgsjd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvqjbeyv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/goooovfae.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujzjdojm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gcnapjeom.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotqqpmhx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fanxiaobao.xyz/Article/details/gxshihpss.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmohxpqan.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gswyxqxkg.sHtML

[F12] CSV 读写
来源：http://baike.fanxiaobao.xyz/Article/details/gnphqdzbe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnhtvncd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fanxiaobao.xyz/Article/details/glkugcfxd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdixhwag.sHtML

TS:   // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gnoqplafs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwfbhyui.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzeozqmg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fanxiaobao.xyz/Article/details/glsniooag.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpvhimzj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsijyumgg.sHtML

G. 面向对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvihszled.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtvvwnszh.sHtML

[G01] 定义类
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfoxktdl.sHtML

Py:   class User: pass
来源：http://baike.fanxiaobao.xyz/Article/details/gaysmdfqv.sHtML

PHP:  class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhwdjwaf.sHtML

JS:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxohfidb.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geegikaqs.sHtML

Java: class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjraubaj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/gefatnzpf.sHtML

Ruby: class User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gezewslui.sHtML

C#:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqxkdpaj.sHtML

[G02] 构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghehqomif.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemsdqajt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpsmuykc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkcjsnnbj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gyrhxkext.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkbegedh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gchskswpr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxszqiza.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzursicde.sHtML

[G03] 实例属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqejptru.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpcyrznc.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrvskwrm.sHtML

JS:   this.name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqyorito.sHtML

TS:   name: string = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvntjcsve.sHtML

Java: private String name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtklyqbra.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fanxiaobao.xyz/Article/details/gcenjmykx.sHtML

Ruby: @name = "x"
来源：http://3g.fanxiaobao.xyz/Article/details/gtnzsqmws.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/geohgxufo.sHtML

[G04] 定义方法
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfogfbku.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fanxiaobao.xyz/Article/details/gwmmmwbfs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gisrmassf.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/geifnmfvs.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjlvlcikj.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfjyyhvn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/giowzfqbo.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/guujojeou.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fanxiaobao.xyz/Article/details/gpnsvnybb.sHtML

[G05] 继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkcdbafa.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcahaxwv.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdgufpzqe.sHtML

JS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gozdrmxob.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gviubiefl.sHtML

Java: class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gecnzuzrg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqrbbcnj.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqnlpfes.sHtML

C#:   class Admin : User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbfrhntu.sHtML

[G06] 重写方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstprhzrh.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fanxiaobao.xyz/Article/details/gsxqrstff.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvywojabh.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/grikfxuuj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdtnorsrd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gilgkbolj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gookexddp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpitaefv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgcxcana.sHtML

[G07] 调用父类方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxknxzdj.sHtML

Py:   super().greet()
来源：http://3g.fanxiaobao.xyz/Article/details/gpwwlketx.sHtML

PHP:  parent::greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxyiurik.sHtML

JS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrmhhpsq.sHtML

TS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gembhqcjn.sHtML

Java: super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvivkghp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gveshdedu.sHtML

Ruby: super
来源：http://wap.fanxiaobao.xyz/Article/details/gsmkijkwg.sHtML

C#:   base.Greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyubeikb.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggustxggt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fanxiaobao.xyz/Article/details/gojmlkywy.sHtML

PHP:  public static function f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqdgwigr.sHtML

JS:   static f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gcswkxjul.sHtML

TS:   static f(): void {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbpgrpio.sHtML

Java: static void f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gthphfcng.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fanxiaobao.xyz/Article/details/gjyowdsnl.sHtML

Ruby: def self.f; end
来源：http://baike.fanxiaobao.xyz/Article/details/gghlkqmtk.sHtML

C#:   public static void F() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfaxtgkfi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fanxiaobao.xyz/Article/details/gcumarpth.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fanxiaobao.xyz/Article/details/govhiwlpx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjyrrywtm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifgmaiha.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggahchdmf.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gymvyuivz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fanxiaobao.xyz/Article/details/gdgrxoblx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fanxiaobao.xyz/Article/details/glaaoydlh.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gpqltslww.sHtML

[G10] 访问控制
来源：http://3g.fanxiaobao.xyz/Article/details/gnulcamtt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfztkrsbm.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/ghzpmuvzy.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedkvzrci.sHtML

TS:   public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gpxniqltg.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fanxiaobao.xyz/Article/details/grbtiberl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoqzbgnz.sHtML

Ruby: public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/githrawpo.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fanxiaobao.xyz/Article/details/gdginmyjp.sHtML

[G11] getter / setter
来源：http://3g.fanxiaobao.xyz/Article/details/goidwebls.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupxkhpsg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnledqzr.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gabowdreg.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdivmbknl.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfewanid.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gqgzcvxcb.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwzfuors.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwtonnses.sHtML

[G12] 对象转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gyaxjtrff.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gbecwvpdb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpmdbgrfp.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvoupyvz.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqjbkukcj.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiomolik.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gedbiwnxa.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goloedqdm.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gcbwdyybw.sHtML

[G13] 判断对象类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gpreznhkn.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqhtzmqm.sHtML

PHP:  $u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/giaojrdgp.sHtML

JS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhfysbzs.sHtML

TS:   u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gspiudfpx.sHtML

Java: u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqruvqyt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskycghzd.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfgcqzrq.sHtML

C#:   u is User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdmsioqj.sHtML

[G14] 数据类 / record
来源：http://wap.fanxiaobao.xyz/Article/details/gpobecmld.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fanxiaobao.xyz/Article/details/gexxfglna.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fanxiaobao.xyz/Article/details/gmsuhhuid.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkthegdgn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwymkuwy.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grffehrzm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerhbqrxp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fanxiaobao.xyz/Article/details/guwfokqfq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fanxiaobao.xyz/Article/details/gkejyojap.sHtML

[G15] 枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnycblfnr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fanxiaobao.xyz/Article/details/ghtesjwok.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdslrpuzb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrlekadf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gusvbbkhe.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfixvkdi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fanxiaobao.xyz/Article/details/ganxahuuc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fanxiaobao.xyz/Article/details/gmpkvdnvx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbdoofgz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxjfucez.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fanxiaobao.xyz/Article/details/gbgvpfwbf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpiisbet.sHtML

JS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gjfdupwur.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gidjfdxva.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fanxiaobao.xyz/Article/details/gkajgusib.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fanxiaobao.xyz/Article/details/gukdzkevz.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyidmntz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gzlvxpwjk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxfvvxkls.sHtML

H. 异常与错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gffjazwyd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjjnucxbf.sHtML

[H01] try / catch 基础
来源：http://read.share.fanxiaobao.xyz/Article/details/gavmnimgb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpjhrljv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxytdzmfy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwuvnajh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopanuhfr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkycbhtw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gajsuufxd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gewyjsvjz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fanxiaobao.xyz/Article/details/gqljlequp.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyznqlyw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fanxiaobao.xyz/Article/details/gntwscdvf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gafvbyrlt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gucjevwmw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/geyqktosu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrvabxsn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fanxiaobao.xyz/Article/details/gppkrmvug.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fanxiaobao.xyz/Article/details/gamkcuzfs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfepunvh.sHtML

[H03] 主动抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gochhssku.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fanxiaobao.xyz/Article/details/grkuaoruv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/ggjglwgdg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcclpzfn.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gtckzsizm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gxjjdpqrh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fanxiaobao.xyz/Article/details/grhlrejve.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fanxiaobao.xyz/Article/details/gojzvfzcs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimiawaqq.sHtML

[H04] 自定义异常类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gbualwlii.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fanxiaobao.xyz/Article/details/galysxspq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpimebsdf.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/groalayxe.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwouzoztt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fanxiaobao.xyz/Article/details/gsmmfetue.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcjdrary.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjzbwsno.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fanxiaobao.xyz/Article/details/gblwjeknp.sHtML

[H05] 捕获特定类型
来源：http://3g.fanxiaobao.xyz/Article/details/ghwelentx.sHtML

Py:   except ValueError as e:
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjoeisus.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzfvaiyd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gghddpgxg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcuxihik.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggunnbfdy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fanxiaobao.xyz/Article/details/gntbjupen.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fanxiaobao.xyz/Article/details/gjaychiye.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghssnpdkh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fanxiaobao.xyz/Article/details/gzbfiogzy.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxafendnc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklbzrwmr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhdvrrxo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjifwpnxh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxzrumkx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fanxiaobao.xyz/Article/details/gjveegoxq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgnqexje.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gknjotxjg.sHtML

[H07] 断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gshhelgtg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fanxiaobao.xyz/Article/details/gqcbqxyhx.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsbhqkmv.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnshxafb.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjykemilo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fanxiaobao.xyz/Article/details/ggeegsmkt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrtuwiov.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gybehebeo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gqophxcts.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gagazrnwv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fanxiaobao.xyz/Article/details/gwnksqqnz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczrzdyfl.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvmznmuh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtsrmyxz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzgqimqi.sHtML

Go:   err.Error()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmhkifkf.sHtML


<!-- 参考信息 -->