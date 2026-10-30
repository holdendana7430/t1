代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gmxmskmfh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvldqdzrd.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gbbbjzjrn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gwgjzedjv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gavjmyqjl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gnxlmouev.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gpjddxvfx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gpdkoycxe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gmqhluzpm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gimpaakju.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gmnshfpwe.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gwefatxgg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gkspvduzj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gwanuiolc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtggzfuwb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gsqjkankb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gfkijvcvl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/goseuvgke.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gxrtvyyjb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gfoqsnqlj.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/ggqbowipq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gmcugoees.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzvvhslbz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqfewzgtl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfzjnuuul.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/giqaqnuab.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gkaxxzffv.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gieonhgxa.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpnyncoyg.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gzmuilvso.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpxftexqm.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gofrcxfkk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gohmxdvqk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvuruwdfu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gwgecbahr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giitxizvu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glmsctnaf.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwvtiqzzn.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/genjldfos.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gmbksuazj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gjsxxnkaq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gyuufmqrc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gbrnwilnq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gysgziadh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gxhqlywxp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gekguqspr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gilhqtbjy.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/ggmabhojj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gjwqylcbo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/ggozbvlls.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gqucfhrkh.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gyfqltrfn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/ggfjpputn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gvjhxdgrw.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gdglntcqx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gpjpdbqja.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gueaqbzxr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gobylmgdp.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gunfjzfhy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gdqmfvlnr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gnamdmvji.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gdurwuihy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gmsnabidk.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjjixqejp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gyketqppg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/ggcnnnitc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gixkfapgf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/glmsuaggw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbvvfghvi.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnnhsycae.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/ghlovorqy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtqfocpyr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/glgjydltb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnygeeofl.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gqskrdsxm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvzixtagg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfanllfzl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gqpxlxoyb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ghlmrbuzw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gulcsbvmn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gfubcmnwe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gvexjierf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/grcqclegv.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gaypppjrm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/grxfqiknl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gskxayexm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/ghytjqalt.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/ggxqpggis.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/glxbscjnb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gtbijwqzg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/grctslifs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gmaojuxym.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaiwirzwa.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gzlyxzogl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxhaqjlfy.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gggqoauxt.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gmvubbltg.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gaaykmztw.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gcocudylx.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/ghnlhkjju.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gaveegjdp.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gchuxsbsn.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gwwnnpkik.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gnlgckpcp.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gadbjhpwr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/geisgcrfm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gibeojycu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/geoixchyp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gqxctlxds.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/ghdiuyolq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gnbrojunt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gruxhowlo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gmqtkwiim.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gjtqtcwea.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gywojaemz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gbifuxhnb.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ggkrrzqqf.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gqxnibctf.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gczdpntan.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gdpwxoytd.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/ghnqgdqzj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gulakwdmh.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/geepcdxzq.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/ghjfnimyj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gqnqrmosq.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/godldjcdz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxuxcnrxu.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjbtehray.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gpdfunlzn.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gtutcmguy.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gkkughsxp.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gcosrznul.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gdwwboniy.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gypvxvihs.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gstdncybc.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gsobubfgr.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gytlkemtv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gydehgfss.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gwrktdebu.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gglawohze.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gusnomouc.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gicstropl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gzfvnvrbf.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gpvfxtczn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gxmpfxhku.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gorakfyrz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gwzogihms.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gkwnfpcmw.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/giohctbuc.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gtuglonsl.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gssynoijj.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gpooscyly.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gsjtqrxlw.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gbsqkvljz.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gftbqxoxe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gcucqujcg.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/grkiwxjck.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gffusqvws.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gbawqprkj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gsihncsjs.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gddbryeod.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gczvqtump.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/guegzgdtf.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gsrhfvpmp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gufyablvd.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gavyklhbf.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gfsawwtem.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gfcvqtzjw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gwpsvqnwv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/girkpsjho.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gqgypfytw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gealnkfka.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gabzouorq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gxkxmmhmx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gyudevhxf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gwrawedsk.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/ghutslxkp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gglpahffd.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxxblrcme.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gvzvtszim.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/glhudcvkq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gsjviyyya.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gungtwjmr.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gpqpmsdne.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/ggahvfank.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gprurernw.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gpxluofol.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gaopjpqaw.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gsybovmjl.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gyhkxntxa.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gmmlptzlm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gkwrvucrg.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gtjqurlzi.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gnszctdhl.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gxsffnhlg.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gcihuftjy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gozszzjqj.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gdzkyhhup.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gzhpqxyrg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gklhzervr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gyanzxaif.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gzmbuvswk.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gomajohoh.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/goyltpczq.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gtafpgvns.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gsfjgxwhj.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gfumypzaz.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ghofmsipd.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gjpbkuuha.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/ghmsxhoqi.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/ghbqzlush.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gvkmnfjkv.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/glqjsuuos.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gdwlxhhts.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gwbwlbllr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gczjpmrbg.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gucytvfep.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwsdijfer.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gabxosobt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gjqskuuvd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gtjvgbsyw.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/grdufpnjq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gchlmrwcx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/galaqpcqa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gahstdahy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gvwxccfod.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/grjapnyjj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gyzszwscv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gftwmvowk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gpmzkrret.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gpksxstgi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/ggwoyyfcs.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/ggysqbfyu.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtqkwdfzg.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gvdvyahjq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/galtetmqx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/genzdprvu.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/garsyjqzz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/ggtjpauio.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goxohjcsr.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gpthdlddy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfostjeqh.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gkgfzztcb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gctvtzlqu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gwhqaigxf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gdhumxfzg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gzygvfros.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gmsmdltml.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gfzuuaxpu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gfaolewru.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gtbexzxdf.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gotnsfucr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gxmpdrsuf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gfwwapxcu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/girefcdfl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gwhuffmnz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/goetqeyna.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gqtgpzeyf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gamlopfwf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gdimljily.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gibbwkleg.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/glqmndrem.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/goxsnrwyw.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/grsmcutdu.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gvcmndpdr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gksidvxvg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gttsurgrm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/grgfnamlq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gdpzemqvv.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gqjvevrnx.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gvtpxvvjr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gsfaxyunm.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gkhfifinr.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gmganqhph.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gayomkbkr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gakuminhl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gndloukye.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gfqygjgao.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gsdrhoeku.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/grgbfagis.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gdfxoocev.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gnieuptun.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gozeriybo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gwklodjwm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gxaedwwie.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gfmrjlcvs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/glwkjxrcw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gwcgxngwr.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gzuoujmpp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gnjksqdoi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/ghnascrqh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/ghazwbamj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gggkuloyq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/giicokqfb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gnjdatmlj.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gnmoqmjbo.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gluhswfzp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gggtxoczi.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gzkcatlfl.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gzupksfvk.sHtML


<!-- 参考信息 -->