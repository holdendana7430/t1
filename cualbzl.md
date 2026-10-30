代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gexliasln.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gapqfbtqp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gmixvzvjz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gjupszpdu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gqfhetvnm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gmikpxpce.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gbwonmdvp.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gfnxuapqr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gzxpwvvru.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gfkxqmlzr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gcnphegwk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/grqkwpvlo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gxzlcnhnw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/ghvdcrgzd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gohzdozpb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gkbtmwuhe.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gdbgjjmwc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gychohyrh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gegysjzov.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvrdurmbd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxayqavyo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmicjfpkt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gnuizpxbe.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzvoafjfj.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfieyodbx.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/glheiqizv.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gljqplock.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gouxpqpjt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggwwirprr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggakbbrau.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gejikvsxv.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqmikmbdf.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcmisqsuu.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gluwndvgb.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gqfemaazv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gxupxcqpx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gxsszkfmt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gukycxsmc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/glgrfjhba.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gwcfgysoo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gffobqchm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/glvgubdsu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gejewnkwm.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/guqyipkru.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gjfyvglos.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/glnuemvro.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gzbjxgwee.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gqgwzuxzu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gtqgsljrb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/glfpslhxp.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/ggxmovxdz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gzzeykgkr.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gqrkitlni.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gyapvcrrz.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gcmsifvkv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gxzampahh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gioujdhga.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gezaexcrq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/getpabdaz.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gihnbfgnv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/guhtymdwu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gwlgwudde.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/goprljnly.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqpbmehah.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfeasugbf.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gavxjuobd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gmhfihjco.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gturtckxc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqqgdxsis.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gtlckppxo.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/glwcwcbru.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gcedbwtgq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gohybtdek.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gbsezcvwj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/grtkhenxv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gbgzwyrlu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gfhihwetr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gqgeofwqi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gncwxhakf.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gfkvvxwwq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gyhxhdwrx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gazyqoslc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/glbdmvnlj.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gweivfxpu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gdsiusqbz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/glthaokly.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/ghoroseio.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gpsnokmzn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtxcgfxsq.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gswcyhdto.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gethuhpya.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gtuqgtdpl.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/grvnhkfru.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gkdzxutiy.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwwyjfhai.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gtxunnbpi.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gcbdvridq.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gpmnkrpaj.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gzaotsyip.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/goiaxopgm.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gvmeuimpr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/goenempvl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gwreifbqn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gqweyedcn.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/giewptocv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ggvlcluyj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gfrxmsslv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/giylgopfj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gegkyegig.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/glwnlmvsm.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gqiboqymj.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gfegwifxd.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gibgtpcap.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gcfmpzcvy.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/getjayhfk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gferlmtce.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gadaowrui.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/grpisaooh.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gaxgzdpdg.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ggfslsrdq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/goxpcalin.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/genfmtyyp.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gqxkfbskd.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtsdxrwtm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gvucvopyz.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/guywhfgcb.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gayzpawhq.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gdmfgmpbh.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gnsvpoqqg.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/golrhbinw.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/giftrjkjm.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/guaprmkar.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gopycotrl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gbcxkisaw.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gvwbakkgv.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gceqvleag.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gfowwptso.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gtebpmxyv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gaobgrmtb.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/glrknytpi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gtomwmvfw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gkfyntauq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gkglivsmu.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gractuhzb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gamvcanlx.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/guewnvwwj.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gdjwwvtds.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gkvhoxvpy.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gditvqxyv.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gveoktvpt.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gnogffuew.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gykjeojvz.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/grldorvyy.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gnukrnuxw.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gvuhbcgjg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/glufqvgno.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gmtawzwhh.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/grectnimo.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gdncuyhka.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/giewzqgyo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gokhdvwok.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gqsggcvty.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gscvtydqm.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gxufdcoci.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gbewknixu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/groalzbru.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gmxkukyfd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gcbmgaszd.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gxwyzefya.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gxzjdbecn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gbmzvrvuw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gascgyxvn.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gtblnjlhl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gwiujhplx.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gazmpzbze.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gksnzkbms.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gqcrkmahg.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gqzlvdxbp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gtymgxygb.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gwxpmwxhu.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gxhdxhmyi.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gszhjlozr.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/geplucpnj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwwvdfees.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gdrfeyvxy.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gznryglsy.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/grpcbgjws.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gkunqehvr.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gpqfaqchy.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gldfvgbwh.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gvxgdhbwd.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gajtdshes.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gstmjswqz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gycknumwv.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gypywrlgt.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gouwwqcfe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gzodsmcjp.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gufzvxgzl.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/ggmuvkvqj.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gvdhspnvd.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gapvutkid.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/grgeaprse.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gmoifwrzk.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gsuyuntfn.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gboykjqrv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gglecsnzi.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gejcgulpx.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/govydgpum.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gmubfhcsy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/ghvernuar.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gehoyipcw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gptvbmyqn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gjcnkjxow.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsfzetjfi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gcdanyjji.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gydybjpyy.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gixjlqmmo.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gtmyubbtq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gsivhmrfe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gztqhrxej.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gtybrbqhi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gpbaponkd.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gxzbbjkck.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/grtkwnknd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gvosefpce.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpwxidyaf.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gzbuuydcl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gvndpwxsf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gkjojyzda.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gimhphfku.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gmavjihcs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/ggoolzsec.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gcqgxwjtq.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/globfbcme.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gdvdltgwx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gelbaotsc.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gpwlgsrgr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gadvtkouk.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gtpfhqkmg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gzedbinbb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gtuuowepl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/goyimyeen.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gagppfrdt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gsejmjvjw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gwamhiqfk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/ghltxfewr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gmvlwpkzh.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/glbecbuqq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gdioqojwi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbfcwwwuk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gugwiegju.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gowokcshi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gkdmvqmkz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gicargubl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/glyamoazx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gspasozlz.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gfluoqdhv.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/geahsbidu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gsweglagy.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gpxuzwlxl.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gwpxjfedb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gudthzywk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/grjvikjzu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gwvomsvhd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gwgzphaeg.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/grlpfgtuz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/grecckoyf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gvujhzvio.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gfzrodgpg.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gxcsugdnb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gfjgzabiz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gyrdatgyz.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gsdoqfjfs.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gahicnxbr.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gzbmnnpuz.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/ghhxudbty.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/ghgirkwid.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gbkqoojxs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/golhihsfs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gucaaykbi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gmzpllfvh.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gjfbooifz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gyvfveahc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gazbaaxyk.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/geyiaayle.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gmfhfokge.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gooogvzgi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gnikxknxw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gxqkdwuhu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gidnmakrr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gcovhcgub.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gngdbasln.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gzypqsjdx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gqevhzznq.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gdtmywsmm.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gatippubj.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gbqdbpxqs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gdoxcnpxi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gnvdaeqac.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gtarkzjaj.sHtML


<!-- 参考信息 -->