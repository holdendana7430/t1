代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/glghqyrtq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glwsyeryn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/glpzwdpji.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gzkaqmxsj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gzwjhjhau.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/glzvauzth.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gcyxbnbxv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/glnojgiie.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gphapzdyx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gtyvmpspe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gbsjbbdpz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gqkkqxohq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gmpblvepx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gmfsyybpk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/guiyhfkkk.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gxgcrfdet.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gwokhlbjm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/giyamdzii.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gyaweglvz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gaeegnoab.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gwrjuvlzi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/geicpyzan.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gdqmrctvu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gtxnxosgl.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gktwpndfm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/ghglgmseb.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/grpuubtbk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guxrnkfnl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqgiaeynq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gderhraup.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gmeitlsbc.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghlcnzony.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gunifnren.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpnliontc.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyydkovxa.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gthkdxhlz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gffheuqch.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtwvsseay.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkvilqoxq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gffyixlow.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvuefqkdn.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gawxhowlw.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gjjnazwxf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gvjjzdujy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gyejftpwn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/golnxbojs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gmzyrfecz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/giqnmkzmk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/ggfrflkzq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gqocatwie.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/goukvjyxj.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gydjscpnf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gmubcbehd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gvqbombby.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gshmiqbcu.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gdsrdqrec.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gxjyjzpqo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gotkuxcmq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gijbcusxh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gebmrilsw.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gcdhpsiqc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grphelwgj.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/giaptteqq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gpekabpqh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gvrfvneee.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gboolixgi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gklvoixqp.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtqecgehy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gmlopsakv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gsxbpjzqq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbrvnqtir.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/glwpnshjx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gucugxgwm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxintyppg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gvhdxogjf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkfsxatpr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyszeerwd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gfkutirrq.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gansksiwo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gkcxmlfpy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/giwsnhnfy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmvrdylrs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwrvndexw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gfotvxddl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gkbvxkpai.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/goudtlufc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gdkcqvlsk.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gdnavogvp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/geuioswlq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/grhzmswxr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gkqzlixlk.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/glfosohfp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gixyfedve.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gcdnlmtfl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gvdxjyfib.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/ghvngbagd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaqldeayf.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gicfxzkps.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxgqaaejr.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gupjxwwxz.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gagghprpd.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gvzyixpon.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gdmwcakws.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gxbeuctyn.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gsdwefemk.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/googdgcgv.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gnffwjxec.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gbrqmfsmp.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gelqftwko.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gaudhgetl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gfswqozur.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gaehdwqfh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcaqikyai.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gidrpwffy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/ggwmmcizg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gtgbjlpbv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gzunvelvb.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gbflnwghh.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gkxujpovm.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gwvvqapuc.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gifjppgzt.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/giqvvhgmw.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gvrzhaqbo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gncberyyy.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gewzamcsr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gpyiqhpez.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gyuzgknez.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/galqjskqt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gqedskbbr.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ggycbkpor.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/graqkplii.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gtnonzxqi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gfazrtgjk.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gaehnndct.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gylycinvh.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gtutmvygi.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gszfwggen.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gpywzmqir.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtdrrhfmc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gkpbwbxnn.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gydjzszbv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/geprjmkum.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gdthklcnc.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gpmujshia.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gderyektt.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gvcnuvjib.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gcmobcwqs.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ggapcjqqt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/glawxhfam.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gghamphib.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gzfwtvzqb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gnjujnoxi.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gsjbbdrqq.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gxupkyhrq.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gbauvjweu.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gzrtckwgh.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gkihhyjtq.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gaewytzxu.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gyzimrgoj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gqvudjubf.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gafdttgtx.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gxzdgzyfu.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gpsftriof.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gsxbzdoww.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gqpkzzttf.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gffwdjmfk.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gxzzscnja.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gyurqkjyz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gwlrtkzdg.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/grnfuaqka.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gvgzazatr.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gcxnhcvnn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gsrofkjqs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gpdsjsftr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gotrhdcgi.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gktisvgpm.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gjoxrbjvx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gfzpfdfpn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gpzmwgbog.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gkzbocafo.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gclocmhuc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gqxsfzfqt.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gozefyrss.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gxznybrrz.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gsbzwhvft.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gmkkdcuuk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gvbqhacru.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gjsqsajzz.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gvvcfbpgs.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gnlfwltjq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gbjzhlntr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gvzcnryjb.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/ghfizowoc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gfdgevsgr.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gxjqsozju.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gcstoahki.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/goxtjaxoo.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gabtwuftw.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gfzffhmgt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gishkzanv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/geweiddig.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/glowaroni.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gxjfzmoqk.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gevhvdtqm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gpvenkmbr.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gxiypeqop.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gbxkvkssx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gtazmdxzr.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gwiozokez.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gmfazjycy.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gtssiuiie.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/golfxvoxu.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gpenostvl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gdvilbsbl.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gborsalql.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gxxuprjvh.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gkxogxxyj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gqjrkffyz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gcnnouazn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/ggvbzasrs.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gnerfxork.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gvatqxglz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gqawcouli.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gypxqnaek.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gdnwfciru.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/guiibylxp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gdqibmwxl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gxnoebppl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gwjaupgad.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gvfqvkmiu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/giebzyfze.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gtuneuvfy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gpmbuekzm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/ghyenbaqf.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/geaquhblp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gxrryorih.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gwpzfghsj.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gvupzzfly.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gpytqnpla.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gboziryrn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gbuvoqhlk.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gnughyrsf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/ggdexjakm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghtdzrzif.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/glyqxuhcg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqlciciww.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gzjzxhbit.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gnszeixxf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gsdkazsyr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gtbtfyeyo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gceldwhjs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/ghdzkwymf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gnegjikww.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gajqgjghn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gccxkhxxi.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gzmhgtzvi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gibdbvdaf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gznhjuyee.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gptykrkim.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gccofdqto.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gfngdjpwd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gvvlmeazb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gprdzkggn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ggnrehnjl.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gvxupgzdh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gcxbqvqtn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gvrfdlrnh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gwometryl.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gbnkakwyl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gtfpuzsuv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gfuxalgro.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gnxejotfw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gfdjnbayh.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/grrdnfoth.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/glemymzvx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/geibhfevc.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gstsayoau.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gxscymldr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/givnneqbp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gauodupzv.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gpsujjmkg.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gmdzthyal.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/grptkiyit.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gnvxcahay.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/ggndbsink.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gmmrojhsk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/geimajvbb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gnzprjfmu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gxyzamcrx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gqmwtmhxb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gaejdqeay.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gmnzbauiv.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gjbhkrapj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gereiyxij.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/guehoddil.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gavlphfth.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/govttagbp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gawwzykyj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gsgvqsfdy.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gpkjvlhqh.sHtML


<!-- 参考信息 -->