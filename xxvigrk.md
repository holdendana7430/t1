代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/giedllraw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gevgujzyf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gdbebmspd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gmhlkjdcw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gdcmfsuci.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gaebpyubg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gojjunxqz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/ghrscfknv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/guugiynjk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gltqibspw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gczhhfpgi.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gbwkrymsl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gjralaxyj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gflgbgnam.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gthcolviq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/ghpsmyeua.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gjmmabvit.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtpbrgxmj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gamkgtzyz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gtrxhdozb.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gciqkcqyq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/ggqwaivxf.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnrfmtlfi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggzcozuyr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjdoprmyx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/glaxmorpa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gewteoccl.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjwogufin.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfjbzzaac.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/ghjeovbst.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnhxbghtu.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqzcodtku.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcndsktka.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzsuupeop.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ggqkgusuc.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gowgygvjm.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxyqqbhon.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxomqatdg.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gcaetxvaz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gmnbxzfuc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gishawhbu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gdfqjwybz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gtzglntvg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbhwyejuh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/glhopbgmd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gkzkzxldb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gjvkiexwo.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gmrtszysl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gtvlahfbf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gpkzxubui.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gejhlrwwj.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gmtqfoukt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gulkmgmgo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gpdnzijwh.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gliznyzlv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjfovkuxf.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gckjcclwr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyjkspetb.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gqlrfzxam.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gvcymxuoa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/ghvfjwvou.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gnmepbyer.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/goyuttnha.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdmfznetw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gcmchewkq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gntnnzikb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpvpxyisv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqvohxrln.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxslgbnax.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfeluxwjy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gdrhaoheq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gjulvhbvp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gclnrspvd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtgkrazdm.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gebgtsfol.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/grfmdocpp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/ggquuysom.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdwhvebng.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvztjhnnn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/guyvvldtl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gtmbnosia.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gnazffnsa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gjdmbztco.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gwxszteza.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gieagtell.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gjwlrrene.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gdqgcvied.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gvooulcvn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/glfrujgvg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/ghesrbxbu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gvnovwwws.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gfvmpbrlt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyvjeyeua.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gjmahwbqv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkputsbvg.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/ggymkuteb.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gtfbsflfp.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gvisojegr.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/grzzdbryz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gpyvnwjds.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/goxekzokb.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxvvyvgx.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gqgnltcer.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/geulxcqrg.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gresawtjc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gyqlgizwj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gsuemsyej.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/ghnwnxvpu.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gtputrvvg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/ghcvxfayd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gekjsyjlt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gpajonkmc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gmgnybnys.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gdynskvue.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gypakxccm.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gqygvnrlf.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gpbgxjwop.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gixombwjk.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gpevwnvpj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gnvbovrkw.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/glvmmvtxn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gixbaqcke.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gknxnzxro.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gobqhhmdm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gevprckmd.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gpqhgfbtz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gfrafvxyl.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gicbdqbtx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gmiucegfc.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gkaxehoqw.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gavrnjvbe.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gvnajsain.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gnrofnjyk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gukeevdxm.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/ghxuiwxxg.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gbtqlafhd.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gzyapftgc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gqqssoxxf.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gmkyqvfxb.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/grfkwtiac.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gcfrrmzmh.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gmyhiuziz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gzibhyhvl.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gyvrmfmvg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gyhjxffxm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gxjfaqhmv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gykzuevov.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gewdzwtpf.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/ganqduuso.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/ghwcxkvxd.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gcmjptnna.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gusylhogl.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/glanvzygi.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gsmnfyzwp.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gsemitqou.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gqqlkzxok.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gvibvcofj.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gyniziycq.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gsshuojwl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gnrvysics.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gmbuekbmr.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gmpyblixy.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/geiqmimdd.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtdawzhqj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/ghumfsjqi.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gpyjnggdk.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gsuijwxic.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gppwehdnd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/ghirjplnr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gwexiwfid.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gtheueyba.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gthzvwque.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gvjfuqsim.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gjkdaucno.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gzliwcjpc.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gdilcvvev.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gbijdaiml.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gyjnkkzof.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gatdbmpkb.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gjjhasscw.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/geobhgzfu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gbofcmdrq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gcygwvowe.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbnsrgc.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gjvqcpsaz.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gpetdfmql.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gwqbbyrxn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxmyufwuc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gqprwquop.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gaugvemyh.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gzxxpjmip.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gpsmpmvtm.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gnzzouibn.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gaiplqfxi.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmovhrjqg.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gqlaiyidf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gyihlhfgf.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gwxdswnar.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gwmsfiqlu.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gtnolprev.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gsjwghrvu.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gysbrolkn.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/ghvqsuysk.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gppbrkyjq.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/goytcgmfv.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ghhljgedk.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/giierjpyu.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gbsixiefu.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/ghoyolwjj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gaqkzhipv.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gddibqsrr.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gfpmwwyoe.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gwpliyqah.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gcmkqysyp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gqbtqjhqa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gesyjhkyl.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gslcasxmt.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gqqabfknf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gnibiwvrd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gtupctbno.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gexgseoar.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gscxmxgzt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/grlfzxyrj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gjxsmwvnm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gjshhhcer.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gvgdhwqbz.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gjgjshslt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gvwrqsorw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gtziotvjj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gpinlmaob.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gbtfjpbyu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gfmybrdug.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/glinbwnax.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gvtsdxkqs.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gnykppiky.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gxsjxavsl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gunoxuvoi.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gqorztjjm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gtgytjeig.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghseqlpxb.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gmepfsagm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkmhqznwc.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gvgpjlgjq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gqjuyjqqq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpctszibs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/geoqbrzpx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gnzfmbgrg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/grzuhpkqo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gcbthwsys.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gvragrmyj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/ghzcvqpas.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gomyezbiz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gtfxdigci.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gdddzwhgu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/guwvwutur.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gcnucrfwv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/guypszhwd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gurzirbpa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gxtrfxhma.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gmlruxexe.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gnujjuqbc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gemhrlqxq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gszopjqnu.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/grzhqijgy.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gctpjoduc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gfhahytzc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gtoumhwfm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/ghxiycnti.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gvlloocwm.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gikeklblg.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gdsfegfwe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gjejfnjgy.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/geqschrog.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gagtxxfsp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gvilijrlx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gebpgezrc.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gmpdvvouc.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gkvwmpofa.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gjbluveay.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gbglyrijo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gzoanqjxi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gvzimmjuz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gyiacvayb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/ghubzijhh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gswjkdmvu.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gunoqkpxr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/ghinkwoto.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gkpxgzlbd.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gtmgvypmd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gcgaeqflg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/geithhrqa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gbuqhxfuy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gguxekcma.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gacecauih.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/giqugvluv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/glnvquppp.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gzhcjolfi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gmaitrleb.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gmtriyrgr.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/glnxcnnzz.sHtML


<!-- 参考信息 -->