代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gjiejwygu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gwphxrwmq.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/glxcpoigg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gtzpzhkhq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gugbcneoi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gcooejmsa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjuyofbod.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gvajkwllr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gaihtvsin.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gbsmdaszc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gzzjborto.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gbhtsxqyj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gbuhnrccb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gwbthsfbm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/ggvykcaxw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/grpkgerhw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gqzjpqhpy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gpiphoety.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gixjujqjy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gqmcrmpct.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gnyqvxhku.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gqqbiejhy.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggwwgrqct.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guwqieygp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzozzzqal.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gedmxsoib.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gyxhajxqi.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gljukqhea.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqulxogit.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gindmdwlw.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzhqecolt.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gdstisplw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gymzpomdi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbnuyzqrw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gyznmlmsx.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggmupipfu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gczwsfybu.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghoyfqyql.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gpgtrwyoh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gkfpxlmlw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gfdsdcqqn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/ggzvpmzdz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gsvedrglv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gjrgloeum.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gtjjsehgn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gmbhrbtzn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gdsmfkgjy.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gicykcmrm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gzktbjqgo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/glbchrxwu.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gwsaosjyg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gwrzthyhi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gagmvdxkn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gazxjxtnu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gobuddcgp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gezkqvhcq.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gdcbczjjo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glzouqirx.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggrnjbmla.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gpddpqkhe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gyrflmgrw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ghdugmkoq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gotwdemlh.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gghtszjrj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/geyauztob.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gzqrdhlsy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnxidjipz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gkjtngxzm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gpwxsbsxl.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gykdivzvd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gfojneemv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gezcqhzhc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/garnmpzyx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gybemqqco.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gozfcxpse.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/goqnqbyra.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gufxamkih.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gpvgfbebp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpiddvefw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gnhrfvtxb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/guegtrsst.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gvzpprcxe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/ggimxcdjo.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gsbwdjvil.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gvsbixnag.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gshefysvg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gzpethjlp.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gbdobohzq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gslejdmyj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gzfmfhvep.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gsyokjwmr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gbfwqkuit.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/galywuryq.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gjdnottfk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glmnpcszg.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gkxddecke.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gzzujlftc.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gytalmmsy.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gttnftbly.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gkskvbeiy.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gwvwyeufy.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gwhsacwyg.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/glbdxbsjn.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqxxvrlfw.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gbsftmqos.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gqtetewfc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gsnjmcssh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/geswgxcdy.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gsrvmxagx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gtihawems.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gqxuxbzfw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/grhdkewix.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gfcgfatna.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/ghfakgpxo.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gbciixinr.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gqaxnsgda.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gekjapkzf.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gswhrjuiy.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/ggoexwsts.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gfewegkno.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gkpucyxri.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/guituriog.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gunjhuxao.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gheyzjdam.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gxiqoaqgu.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/grgwztmfu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcegbwde.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/grurmixmt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gjdfryero.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/ghbuxieyj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gpfpdgvsu.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gzvtanvnw.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gspjucqbh.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gckxblgif.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmkovupmr.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpuanwhmi.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gudamblpe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gtaeemnyv.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gqgmfyxsd.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gmpzmufnn.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gxggbmlvo.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gqadyrxny.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gclpgfuyd.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gasyylujk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gwtyhoumw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gpqapjghb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gxadlvpyt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gsnsjwxax.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gejzfquss.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gkynqzhxn.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gxtghnagf.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gpzxddcsi.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gvgzdctwj.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gibwjgfsr.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gqlrmocxu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gzgcqqrsl.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/goaargdvh.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gjrpohftg.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gsrwinxax.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gaauevcqd.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gykfbtalv.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/ghmgpmoio.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gmtpekfhd.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gxaalrksg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gvljeoitc.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gscesnuan.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/glxszkwgt.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gslqpssyc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gbkdxgtpq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gqflgusjs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/grlanlwzx.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gbxeiyjap.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gxyhvnzbn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gnbuqvewf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gseicmjdo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdwpfxayi.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gixmgclgw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gxdjbphsh.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/grkhvecpz.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/ggqbfewdb.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gbxzoljby.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gmchdeeya.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gboicibec.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gwlyoknws.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gnjqrvjuv.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/glrxfmujv.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gbssbjiwh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gfkxippqu.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gfawnzlfh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gmmtcfaeb.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/grpfocrgf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gsbhwyqks.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gmbqwtitj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/ggxzvlahc.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gbnvexrlm.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gyquwteqb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/guqzbbyea.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gjfmkybvh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gsdggohkb.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gtcfhbwnj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gzkuhhnjm.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gbmjltcii.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gdrivmnqn.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gefmvgpmy.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gcwmsatzv.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gqeiuylkr.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gjsgkjzqq.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gcarecvfh.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gkljukkin.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gzkrpifby.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/giaaceefu.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gqndmfpgp.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gubclwmew.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/grglagscy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gtjsvctlo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gkmnqgckv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/ggeixgnpr.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gntztercb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gyleqxzla.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gjuwkdcdk.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gwcrxedfo.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gacfdhodx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gavxcwjvk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gjykpfism.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gicnvolnx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/guomvkawp.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gjloppovw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/goybovpiz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gvnsrdsuc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gmexqopve.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gifcothzo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/goqztrgzm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/ggufqseww.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gbtsmrpoh.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gkckpbcwb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/grlfbuayp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/grdgtcrkv.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gvagsdfvh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gydtinpgl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmwtutzyy.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gptvvdimg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdduukaec.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gpspabjea.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gikevqvoe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggqjeahhq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gzsvagjzg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gijidwvnn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gpvthuyte.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gvzvmobhg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gqzgavyrj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gcwjcakvk.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gjnhpyfrv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gjzieyidu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gbsiqjzzy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gelvnoveh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gwtqcenmc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gfcqfghbx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/ggvylmiie.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gvhyowlbs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ggkusxjyb.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gllpiktml.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gvnlzozmp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gklghqopf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/ghcrkddrj.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gbtwqolda.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gzggggvca.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gssdczgoq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/glheugjxw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gbfsffenq.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gbrbrsrjc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gvuuswsyt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gfdgrctsx.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gxehniakg.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gfaqpeuit.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gelmlrtyw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gaojicdzu.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gxhkupecd.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gltmpkezp.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gwunycjdm.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gpegivtxc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gchkswczc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/glifxeaiz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gfelwlrtr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gwsjbfqoe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gjjykplba.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/geglbriou.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gapinwtri.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gnwdwcfkx.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/ggugewoob.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gxoashdku.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gnuzaiqel.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gmakcvwbn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gpjbidnkc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gpvdkdnoo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gidgufbyu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gqwjsrdmg.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gsawksrfi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/grllfozjq.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gkrtempzg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gtlndvgay.sHtML


<!-- 参考信息 -->